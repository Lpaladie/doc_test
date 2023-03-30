# Расходные кассовые ордера

Для регистрации расходов наличных денежных средств из кассы организации предназначен документ **"Расходный кассовый ордер"**.

Документы **"Расходные кассовые ордера"** расположены в разделе **"Деньги"** - **"Кассы"**.

[![1][1]][1]

В документе заполняются поля:

- Номер - заполняется автоматически при сохранении
- Дата
- Вид операции - влияет на состав реквизитов документов. Возможны 5 видов операций:

    - ***Возврат оплаты клиенту***, в документе заполняются реквизиты:

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

    - ***Прочие расходы***, в документе заполняются поля:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - Сумма документа
        - Валюта
        - Дата платежа

        [![5][5]][5]

    - ***Выдача подотчетнику***, в документе заполняются поля:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - Подотчетное лицо
        - Сумма документа
        - Валюта
        - Дата платежа

        [![6][6]][6]

    - ***Списание по результатам инвентаризации***, в документе заполняются поля:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - [Инвентаризация](CashInventory.md)
        - Сумма документа
        - Валюта
        - Дата платежа

        [![7][7]][7]

    - ***Инкассация в банк***, в документе заполняются поля:

        - [Организация](../CommonInformation/Organization.md)
        - [Подразделение](../CommonInformation/Department.md)
        - Касса
        - Банковский счет
        - Сумма документа
        - Валюта
        - Дата платежа

        [![9][9]][9]

Для **"Расходных кассовых ордеров"** со всеми видами операций заполняется вкладка "Печать"

[![4][4]][4]

и может быть распечатан "Расходный кассовый ордер"

[![8][8]][8]

[1]: CashExpenseOrders.assets/1.png
[2]: CashExpenseOrders.assets/2.png
[3]: CashExpenseOrders.assets/3.png
[4]: CashExpenseOrders.assets/4.png
[5]: CashExpenseOrders.assets/5.png
[6]: CashExpenseOrders.assets/6.png
[7]: CashExpenseOrders.assets/7.png
[8]: CashExpenseOrders.assets/8.png
[9]: CashExpenseOrders.assets/9.png
