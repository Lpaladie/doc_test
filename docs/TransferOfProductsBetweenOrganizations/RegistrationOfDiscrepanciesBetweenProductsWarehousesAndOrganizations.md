# Оформление расхождений товаров складов и организаций

Для оформления документов **"Оприходования товаров организации"** и **"Списания товаров организации"** используется обработка **"Оформление расхождений товаров"**, которая расположена в разделе **"Заказы"** в подсистеме **"Внутригрупповые обороты"**. Документы оформляются для того, чтобы все товары на складе были поставлены на учет в той или иной организации.

[![1][1]][1]

После открытия обработки заполняются поля:

- Организация по умолчанию - та организация на которую оприходуются/с которой списываются товары
- Вид цен для инвентаризации (вид цены должен быть без включения НДС)
- Дата
- Отборы:
    - Склад
    - Организация
    - Номенклатура

Затем нажимаем кнопку **"Обновить"**, на форме будут выведены товары на складах, их количество на складе и на организации, если есть недостатки/излишки, то строки будут подсвечены красным цветом. Для списания/оприходования товаров в организацию переносим товар в правую часть формы. Далее необходимо нажать кнопку **"Оформить документы"**, чтобы сформировать документы *"Оприходования товаров организации"* и *"Списания товаров организации"*.

Смоделируем пример, который демонстрирует работу АРМа **"Оформление расхождений товаров"**.

Создадим новый склад на котором ведется учет товаров по организации Сырная ГП:

[![2][2]][2]

Создадим вид цен "Цена оприходования/списания для Коровки" не включающий НДС:

[![3][3]][3]

Создадим документ "Установка цен" от 18.06.2020 для вида цены Цена оприходования/списания для Коровки, установим цены для номенклатуры:

- Сыр Адыгейский - 100
- Сыр Костромской - 150

[![4][4]][4]

[![5][5]][5]

Создадим документы *"Распоряжение на приемку"* и *"Распоряжение на отгрузку"* для склада Сырная ГП:

- Распоряжение на приемку: дата - 18.06.2020, Сыр Адыгейский - 10

[![6][6]][6]

[![7][7]][7]

- Распоряжение на отгрузку: дата - 18.06.2020, Сыр Костромской - 10

[![8][8]][8]

[![9][9]][9]

В обработке **"Оформление расхождений товаров"** заполняем поля и отборы:

- Организация по умолчанию - Коровка
- Вид цен для инвентаризации - Цена оприходования/списания для Коровки
- Дата - 18.06.2020
- Склад - Сырная ГП

Нажимаем кнопку **"Обновить"**, на форме будут выведены товары склада Сырная ГП:

[![10][10]][10]

По данным товарам не ведется учет ни в одной из организаций, Сыр Адыгейский необходимо оприходовать в организацию, а Сыр Костромской списать с организации. Перенесем товары в правую часть формы и нажмем кнопку **"Оформить документы"**, чтобы сформировать документы *"Оприходование товаров организации"* и *"Списание товаров организации"*.

[![11][11]][11]

Проверим, что документ *"Оприходование товаров организации"* сформировался корректно:

[![12][12]][12]

[![13][13]][13]

Проверим, что документ *"Списание товаров организации"* сформировался корректно:

[![14][14]][14]

[![15][15]][15]

[1]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/1.png
[2]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/2.png
[3]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/3.png
[4]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/4.png
[5]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/5.png
[6]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/6.png
[7]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/7.png
[8]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/8.png
[9]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/9.png
[10]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/10.png
[11]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/11.png
[12]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/12.png
[13]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/13.png
[14]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/14.png
[15]: RegistrationOfDiscrepanciesBetweenProductsWarehousesAndOrganizations.assets/15.png