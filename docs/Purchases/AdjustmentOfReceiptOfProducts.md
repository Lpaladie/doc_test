# Создание корректировок поступлений товаров

Для внесения исправлений в документы [*"Поступления товаров"*](ReceiptOfProducts.md) используются документы **"Корректировка поступлений товаров"**. Они расположены в разделе **"Закупки"**.

[![1][1]][1]

При создании документа указываются:

**Вкладка "Основное"**

- Номер - заполняется автоматически
- Дата
- Основание: поступление товаров или корректировка поступления товаров. Документ *"Корректировка поступлений товаров"* может создаваться на основании *"Почтупления товаров"* или другого документа *"Корректировка поступления товаров"*
- Вид корректировки:
    - Исправление ошибок
    - Корректировка по соглашению сторон

Остальные поля формы будут заполнены автоматически по выбранному основанию. 

**Вкладка "Товары"**

Заполняется автоматически по основанию, на ней фиксируются все изменения, которые произошли в поступлении товаров.

**Вкладка "Расхождения"**

С помощью кнопки **"Заполнить расхождения"** табличная часть заполняется расхождениями между документом-основанием и данными внесенными в табличную часть на вкладке *"Товары"*.

Создадим корректировку для поступления товаров, которое было создано первым по заказу на 24.07.2020

- Дата: 27.07.2020
- Вид корректировки: Корректировка по соглашению сторон

[![2][2]][2]

На вкладке **"Товары"** вносим изменения:

- Сыр Адыгейский - цена 180
- Сыр Костромской - количество 7

[![3][3]][3]

На вкладке **"Расхождения"** заполняем с помощью кнопки **"Заполнить расхождения"** расхождения товаров, указываем причины корректировок - создаются в справочнике **"Причины корректировок документов"**

[![4][4]][4]

Сохраняем документ, нажав кнопку **"Провести и закрыть"**.

[1]: AdjustmentOfReceiptOfProducts.assets/1.png
[2]: AdjustmentOfReceiptOfProducts.assets/2.png
[3]: AdjustmentOfReceiptOfProducts.assets/3.png
[4]: AdjustmentOfReceiptOfProducts.assets/4.png