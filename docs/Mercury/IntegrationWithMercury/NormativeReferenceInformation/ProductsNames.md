# Наименования продукции

Справочник наименований продукции заполняется следующими способами:

- В веб интерфейсе и потом подгружается через АПИ в 1С, после загрузки дозаполняются реквизиты
- В 1С. После заполнения основных реквизитов через АПИ присваивается ГУИД и после дозаполняются необходимые реквизиты

## Загрузка из ГИС Меркурий

Предварительно загрузить наименования, ранее созданные в веб-интерфейсе, можно следующим образом:

1. Открыть **ГИС Меркурий** - **Сервис** – **Управление Интеграцией с ГИС Меркурий**. Откроется обработка с настройками Меркурия

    [![1][1]][1]

2. Открыть вкладку **Классификаторы** и выбрать **Наименования продукции**

    [![2][2]][2]

3. На вкладке **Импорт** указать производителя продукции и нажать команду загрузить. Будут загружены в временную таблицу данные с сервера Меркурия.

    [![3][3]][3]

4. Необходимо выбрать подходящую номенклатуру (с помощью клавиши CTRL можно выбрать несколько позиций) и нажать команду **Создать элементы по выбранным строкам** (синяя стрелка)

Наименования продукции можно загрузить по ГУИД, также они подгрузятся с ВСД и записями журналов.

[![4][4]][4]

## Создание через АПИ

При создании наименования продукции заполняются поля:

- Признак собственной продукции, если не установлен – справочник не редактируется
- Наименование, Полное наименование – обязательные к заполнению
- Артикул – заполнять не обязательно
- GTIN, ГОСТ – заполняются по потребности
- Тип продукции, продукция, вид продукции – заполняются предопределенными уровнями ТНВЭД
- Ед. изм – единица измерения хранения остатков, подставляется в партии отсюда
- Срок годности – используется для расчета даты окончания срока годности, рассчитывается автоматически при ручном создании производственных партий
- Производитель – основной ХС производитель
- Собственник ТМ – ХС собственник ТМ
- Площадка – список производителей
- Раздел "Фасовка" – нужен для расчета информации по упаковкам, в случае если правилами заполнения маркировок предусмотрено расчетное заполнение потребительских и торгового уровня в исходящих партиях
- Способ хранения – подставляется в исходящие партии, происходит разбиение по способу хранения, если в реализации товаров есть различия в продукции

[![5][5]][5]

[1]: ProductsNames.assets/1.png
[2]: ProductsNames.assets/2.png
[3]: ProductsNames.assets/3.png
[4]: ProductsNames.assets/4.png
[5]: ProductsNames.assets/5.png
