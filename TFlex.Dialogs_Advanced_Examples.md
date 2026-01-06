# Продвинутые примеры использования классов в пространстве имён TFlex.Dialogs

## Комплексные диалоговые интерфейсы

### Создание диалога параметров вала с валидацией

```csharp
internal class ShaftParametersDialog : ModalDialog
{
    private NumericInputControl _lengthInput;
    private NumericInputControl _diameterInput;
    private ToggleControl _threadedCheck;
    private NumericInputControl _threadPitchInput;
    
    public ShaftParametersDialog(ShaftData shaftData) : base("Параметры вала")
    {
        CreateDialogControls(shaftData);
        LoadData(shaftData);
    }
    
    private void CreateDialogControls(ShaftData shaftData)
    {
        ModalDialogPage mainPage = new ModalDialogPage();
        Pages.Add(mainPage);
        
        GridControl mainGrid = new GridControl { RowCount = 4, ColumnCount = 2 };
        mainGrid.SetAutoWidth(0);
        mainPage.Controls.Add(mainGrid);
        
        // Поле длины
        mainGrid.SetControl(0, 0, new ControlsWindowForm { Caption = "Длина (мм)" });
        _lengthInput = new NumericInputControl { Value = 100.0, Minimum = 1.0, Maximum = 10000.0 };
        _lengthInput.ValueChanged += OnLengthChanged;
        mainGrid.SetControl(0, 1, _lengthInput);
        
        // Поле диаметра
        mainGrid.SetControl(1, 0, new ControlsWindowForm { Caption = "Диаметр (мм)" });
        _diameterInput = new NumericInputControl { Value = 20.0, Minimum = 1.0, Maximum = 1000.0 };
        mainGrid.SetControl(1, 1, _diameterInput);
        
        // Флажок резьбы
        _threadedCheck = new ToggleControl { Text = "Резьбовой" };
        _threadedCheck.CheckStateChanged += OnThreadedChanged;
        mainGrid.SetControl(2, 0, _threadedCheck);
        
        // Шаг резьбы (изначально скрыт)
        mainGrid.SetControl(3, 0, new ControlsWindowForm { Caption = "Шаг резьбы (мм)" });
        _threadPitchInput = new NumericInputControl { Value = 1.0, Minimum = 0.1, Maximum = 10.0, Enabled = false };
        mainGrid.SetControl(3, 1, _threadPitchInput);
    }
    
    private void LoadData(ShaftData shaftData)
    {
        // Загрузка данных из модели
        _lengthInput.Value = shaftData.Parameters.Length.Value;
        _diameterInput.Value = shaftData.Parameters.Diameter.Value;
        _threadedCheck.CheckState = shaftData.Parameters.IsThreaded ? CheckState.Checked : CheckState.Unchecked;
        _threadPitchInput.Value = shaftData.Parameters.ThreadPitch.Value;
        UpdateThreadControls();
    }
    
    private void OnLengthChanged(object sender, EventArgs e)
    {
        // Валидация длины
        if (_lengthInput.Value < _diameterInput.Value)
        {
            MessageBox.Show("Длина не может быть меньше диаметра!");
            _lengthInput.Value = _diameterInput.Value + 10;
        }
    }
    
    private void OnThreadedChanged(object sender, EventArgs e)
    {
        UpdateThreadControls();
    }
    
    private void UpdateThreadControls()
    {
        bool isThreaded = _threadedCheck.CheckState == CheckState.Checked;
        _threadPitchInput.Enabled = isThreaded;
    }
    
    public override bool ShowDialog()
    {
        bool result = base.ShowDialog();
        if (result)
        {
            // Сохранение данных
            SaveData();
        }
        return result;
    }
    
    private void SaveData()
    {
        // Сохранение в модель
        // shaftData.Parameters.Length.Value = _lengthInput.Value;
        // ...
    }
}
```

### Создание диалога с динамическими элементами управления

```csharp
internal class DynamicControlsDialog : ModalDialog
{
    private GridControl _mainGrid;
    private List<NumericInputControl> _stepInputs = new List<NumericInputControl>();
    private ToggleControl _addStepCheck;
    
    public DynamicControlsDialog() : base("Динамические элементы")
    {
        CreateDynamicControls();
    }
    
    private void CreateDynamicControls()
    {
        ModalDialogPage page = new ModalDialogPage();
        Pages.Add(page);
        
        _mainGrid = new GridControl { RowCount = 1, ColumnCount = 1 };
        _mainGrid.SetAutoWidth(0);
        page.Controls.Add(_mainGrid);
        
        // Флажок для добавления шагов
        _addStepCheck = new ToggleControl { Text = "Добавить шаг вала" };
        _addStepCheck.CheckStateChanged += OnAddStepChanged;
        _mainGrid.SetControl(0, 0, _addStepCheck);
    }
    
    private void OnAddStepChanged(object sender, EventArgs e)
    {
        if (_addStepCheck.CheckState == CheckState.Checked)
        {
            AddStepControls();
        }
        else
        {
            RemoveStepControls();
        }
    }
    
    private void AddStepControls()
    {
        // Увеличение сетки
        _mainGrid.RowCount += 3;
        
        // Добавление элементов для нового шага
        int startRow = 1;
        
        // Длина шага
        _mainGrid.SetControl(startRow, 0, new ControlsWindowForm { Caption = "Длина шага (мм)" });
        NumericInputControl lengthInput = new NumericInputControl { Value = 50.0 };
        _mainGrid.SetControl(startRow + 1, 0, lengthInput);
        _stepInputs.Add(lengthInput);
        
        // Диаметр шага
        _mainGrid.SetControl(startRow + 2, 0, new ControlsWindowForm { Caption = "Диаметр шага (мм)" });
        NumericInputControl diameterInput = new NumericInputControl { Value = 20.0 };
        _mainGrid.SetControl(startRow + 3, 0, diameterInput);
        _stepInputs.Add(diameterInput);
        
        // Тип шага
        _mainGrid.SetControl(startRow + 4, 0, new ControlsWindowForm { Caption = "Тип шага" });
        // Добавление ComboBox или других элементов...
    }
    
    private void RemoveStepControls()
    {
        // Очистка дополнительных элементов
        _stepInputs.Clear();
        _mainGrid.RowCount = 1;
        _mainGrid.SetControl(0, 0, _addStepCheck);
    }
}
```

### Создание мастера с несколькими шагами

```csharp
internal class ShaftWizardDialog : ModalDialog
{
    private int _currentStep = 0;
    private List<ModalDialogPage> _wizardPages;
    private ButtonControl _nextButton;
    private ButtonControl _backButton;
    
    public ShaftWizardDialog() : base("Мастер создания вала")
    {
        CreateWizardPages();
        SetupNavigation();
        ShowCurrentStep();
    }
    
    private void CreateWizardPages()
    {
        _wizardPages = new List<ModalDialogPage>();
        
        // Шаг 1: Основные параметры
        ModalDialogPage step1 = new ModalDialogPage();
        step1.Caption = "Шаг 1: Основные параметры";
        CreateStep1Controls(step1);
        _wizardPages.Add(step1);
        
        // Шаг 2: Геометрия
        ModalDialogPage step2 = new ModalDialogPage();
        step2.Caption = "Шаг 2: Геометрия вала";
        CreateStep2Controls(step2);
        _wizardPages.Add(step2);
        
        // Шаг 3: Материал и отделка
        ModalDialogPage step3 = new ModalDialogPage();
        step3.Caption = "Шаг 3: Материал и отделка";
        CreateStep3Controls(step3);
        _wizardPages.Add(step3);
        
        // Добавление всех страниц
        foreach (var page in _wizardPages)
        {
            Pages.Add(page);
        }
    }
    
    private void SetupNavigation()
    {
        // Создание кнопок навигации
        _backButton = new ButtonControl { Text = "Назад", Enabled = false };
        _backButton.Click += OnBackClick;
        
        _nextButton = new ButtonControl { Text = "Далее" };
        _nextButton.Click += OnNextClick;
        
        // Добавление кнопок на каждую страницу
        foreach (var page in _wizardPages)
        {
            GridControl navGrid = new GridControl { RowCount = 1, ColumnCount = 2 };
            navGrid.SetControl(0, 0, _backButton);
            navGrid.SetControl(0, 1, _nextButton);
            page.Controls.Add(navGrid);
        }
    }
    
    private void ShowCurrentStep()
    {
        // Показ только текущей страницы
        for (int i = 0; i < _wizardPages.Count; i++)
        {
            _wizardPages[i].Visible = (i == _currentStep);
        }
        
        // Обновление кнопок
        _backButton.Enabled = (_currentStep > 0);
        _nextButton.Text = (_currentStep == _wizardPages.Count - 1) ? "Готово" : "Далее";
        
        Caption = _wizardPages[_currentStep].Caption;
    }
    
    private void OnNextClick(object sender, EventArgs e)
    {
        if (_currentStep < _wizardPages.Count - 1)
        {
            _currentStep++;
            ShowCurrentStep();
        }
        else
        {
            // Завершение мастера
            DialogResult = true;
            Close();
        }
    }
    
    private void OnBackClick(object sender, EventArgs e)
    {
        if (_currentStep > 0)
        {
            _currentStep--;
            ShowCurrentStep();
        }
    }
    
    // Методы создания элементов для каждого шага
    private void CreateStep1Controls(ModalDialogPage page) { /* ... */ }
    private void CreateStep2Controls(ModalDialogPage page) { /* ... */ }
    private void CreateStep3Controls(ModalDialogPage page) { /* ... */ }
}
```

### Создание диалога с предварительным просмотром

```csharp
internal class PreviewDialog : ModalDialog
{
    private NumericInputControl _parameterInput;
    private ToggleControl _previewCheck;
    private System.Windows.Forms.PictureBox _previewBox;
    
    public PreviewDialog() : base("Диалог с предварительным просмотром")
    {
        CreatePreviewControls();
        SetupPreviewEvents();
    }
    
    private void CreatePreviewControls()
    {
        ModalDialogPage page = new ModalDialogPage();
        Pages.Add(page);
        
        GridControl grid = new GridControl { RowCount = 3, ColumnCount = 2 };
        grid.SetAutoWidth(0);
        page.Controls.Add(grid);
        
        // Параметр
        grid.SetControl(0, 0, new ControlsWindowForm { Caption = "Параметр" });
        _parameterInput = new NumericInputControl { Value = 50.0 };
        grid.SetControl(0, 1, _parameterInput);
        
        // Флажок предварительного просмотра
        _previewCheck = new ToggleControl { Text = "Показать предварительный просмотр" };
        grid.SetControl(1, 0, _previewCheck);
        
        // Область предварительного просмотра
        _previewBox = new System.Windows.Forms.PictureBox();
        _previewBox.Size = new System.Drawing.Size(200, 200);
        _previewBox.BorderStyle = System.Windows.Forms.BorderStyle.FixedSingle;
        grid.SetControl(2, 0, _previewBox);
    }
    
    private void SetupPreviewEvents()
    {
        _parameterInput.ValueChanged += UpdatePreview;
        _previewCheck.CheckStateChanged += OnPreviewToggled;
    }
    
    private void OnPreviewToggled(object sender, EventArgs e)
    {
        _previewBox.Visible = (_previewCheck.CheckState == CheckState.Checked);
        if (_previewBox.Visible)
        {
            UpdatePreview(null, null);
        }
    }
    
    private void UpdatePreview(object sender, EventArgs e)
    {
        if (!_previewBox.Visible) return;
        
        // Генерация изображения предварительного просмотра
        using (System.Drawing.Bitmap bmp = new System.Drawing.Bitmap(200, 200))
        using (System.Drawing.Graphics g = System.Drawing.Graphics.FromImage(bmp))
        {
            g.Clear(System.Drawing.Color.White);
            
            // Рисование в зависимости от параметра
            double param = _parameterInput.Value;
            g.DrawEllipse(System.Drawing.Pens.Blue, 50, 50, (float)param, (float)param);
            
            _previewBox.Image = (System.Drawing.Image)bmp.Clone();
        }
    }
}
```</content>
<parameter name="filePath">d:\work\T-Flex\macros\Source\TFlex.Dialogs_Advanced_Examples.md