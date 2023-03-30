# Приходные кассовые ордера

Для регистрации поступления наличных денежных средств в кассу организации предназначен документ **"Приходный кассовый ордер"**.

Документы **"Приходные кассовые ордера"** расположены в разделе **"Деньги"** - **"Кассы"**.

[![1][1]][1]

В документе заполняются поля:

- Номер - заполняется автоматически при сохранении
- Дата
- Вид операции - влияет на состав реквизитов документов. Возможны 4 вида операций:

    - ***Поступление оплаты*** - фиксирует оплату от клиента, в документе заполняются реквизиты:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - [Контрагент](../CommonInformation/Contractor.md)
        - Сумма документа
        - Валюта
        - Дата платежа

        [![2][2]][2]

        На вкладке **"Расшифровка платежа"** табличная часть заполняется следующими данными:

        - Основание - [соглашение с контрагентом](../CRM/CustomerService/Pricing/AgreementsWithContractors.md)
        - Объект расчета - объект по которому будет зачтена оплата от клиента, это могут быть [соглашение с контрагентом](../CRM/CustomerService/Pricing/AgreementsWithContractors.md) или [реализации товаров](../CRM/CustomerService/FormationOfShipments/FormationOfTheAccompanyingDocuments/FormationOfTheImplementationsOfProducts.md)
        - Сумма
        - [Статья ДДС](CashFlowItems.md)

        [![3][3]][3]

        **"Приходные кассовые ордера"** с операцией ***Поступление оплаты*** могут оформляться на основании реализаций товаров.

    - ***Прочие приходы***, в документе заполняются поля:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - Сумма документа
        - Валюта
        - Дата платежа

        [![5][5]][5]

    - ***Поступление от подотчетного лица***, в документе заполняются поля:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - Подотчетное лицо
        - Сумма документа
        - Валюта
        - Дата платежа

        [![6][6]][6]

    - ***Оприходование по результатам инвентаризации***, в документе заполняются поля:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - [Инвентаризация](CashInventory.md)
        - Сумма документа
        - Валюта
        - Дата платежа

        [![7][7]][7]

Для **"Приходных кассовых ордеров"** со всеми видами операций заполняется вкладка "Печать"

[![4][4]][4]

и может быть распечатан "Приходный кассовый ордер"

[![8][8]][8]

[1]: IncomingCashOrders.assets/1.png
[2]: IncomingCashOrders.assets/2.png
[3]: IncomingCashOrders.assets/3.png
[4]: IncomingCashOrders.assets/4.png
[5]: IncomingCashOrders.assets/5.png
[6]: IncomingCashOrders.assets/6.png
[7]: IncomingCashOrders.assets/7.png
[8]: IncomingCashOrders.assets/8.png
