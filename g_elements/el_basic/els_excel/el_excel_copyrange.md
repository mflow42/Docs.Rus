# Копирование диапазона

![](<Копирование диапазона.png>)

Позволяет скопировать диапазон ячеек Excel и вставить в другой лист. Вставку возможно осуществить как внутри одного документа, так и во внешний файл Excel.

Диапазон копируется в соответствии с форматом, заданным в одноименном свойстве. Доступны следующие варианты:

* **All** (по умолчанию) - будут скопированы все значения, форматы и формулы из диапазона.
* **Values** - будут скопированы только значения. Формат ячеек и формулы будут проигнорированы - вместо формул подставится готовый результат.
* **Formulas** - будут скопированы значения и формулы. Чтобы значение формул корректно отображалось при вставке, добавьте после копирования диапазона компонент [**Пересчет формул**](https://docs.primo-rpa.ru/primo-rpa/g\_elements/osnovnye-elementy/prilozhenie-excel/el\_excel\_calc).
* **Formats** - будет скопирован только формат ячеек, шрифт и цвета. Значения и формулы проигнорируются.

**ВАЖНО!** После копирования диапазона не забудьте использовать элемент [**Сохранить документ**](https://docs.primo-rpa.ru/primo-rpa/g\_elements/osnovnye-elementy/prilozhenie-excel/el\_excel\_save), чтобы внесенные изменения применились.

> _Описание общих свойств см. в разделе_ [_**Работа с элементами**_](https://docs.primo-rpa.ru/primo-rpa/primo-studio/process/elements)

| Свойство                  | Тип    | Описание                                                                                                                                                                                      |
| ------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Диапазон-источник\*       | String | Укажите диапазон ячеек, которые нужно скопировать. Диапазон можно указать в точности: "A1:D12" либо использовать символ \* вместо столбца или номера строки, например: "A1:\*12" или "A1:D\*" |
| Диапазон-приемник\*       | String | Укажите диапазон ячеек для вставки данных                                                                                                                                                     |
| Страница-источник         | String | Введите наименование страницы-источника данных                                                                                                                                                |
| Индекс страницы-источника | Int32  | Номер страницы-источника (отсчет с 0)                                                                                                                                                         |
| Страница-приемник         | String | Наименование страницы-приемника данных                                                                                                                                                        |
| Индекс страницы-приемника | Int32  | Номер страницы-приемника (отсчет с 0)                                                                                                                                                         |
| Формат                    | -      | Выберите, в каком формате нужно скопировать данные. Описание значений приведено выше                                                                                                          |
| Путь к документу          | String | Если данные нужно вставить во внешний файл Excel, укажите к нему путь. Если он не задан, диапазон будет вставлен внутри файла-источника                                                       |

{% tabs %}
{% tab title="C#" %}
```csharp
LTools.Office.ExcelApp app = LTools.Office.ExcelApp.Init(wf, @"c:\file.xlsx");
app.CopyRange("A1:C22", "A1:C22", null, 0, null, 1);
```
{% endtab %}

{% tab title="Python" %}
```python
app = LTools.Office.ExcelApp.Init(wf, @"c:\file.xlsx")
app.CopyRange("A1:C22", "A1:C22", None, 0, None, 1)
```
{% endtab %}

{% tab title="JavaScript" %}
```javascript
var app = _lib.LTools.Office.ExcelApp.Init(wf, @"c:\file.xlsx");
app.CopyRange("A1:C22", "A1:C22", null, 0, null, 1);
```
{% endtab %}
{% endtabs %}
