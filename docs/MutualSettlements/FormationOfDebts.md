# Формирование задолженностей

После того как [график оплаты](PaymentSchedule.md) был создан, чтобы он работал нужно его указать в [соглашении с контрагентом](../CRM/CustomerService/Pricing/AgreementsWithContractors.md).

В соглашении с контрагентом на вкладке **"Взаиморасчеты"** заполняются:

- Признак использования взаиморасчетов для расчета задолженности (в проверках заказов клиентов)
- Валюта взаиморасчетов
- Порядок расчетов:

    - По накладным
    - По соглашениям

- [График оплаты](PaymentSchedule.md)

[![1][1]][1]

В [заказе клиента](../CRM/CustomerService/FormationOfOrders/CustomerOrder) из соглашения заполняются порядок расчетов, форма оплаты, график оплаты и валюта.

[![2][2]][2]

В [реализации товаров](../CRM/CustomerService/FormationOfShipments/FormationOfTheAccompanyingDocuments/FormationOfTheImplementationsOfProducts.md) из соглашения заполняются порядок расчетов, форма оплаты, график оплаты и валюта. Табличная часть при проведении документа или по нажатию кнопки **"Заполнить по графику"** заполняется информацией о том какими датами и какими суммами ожидаются оплаты от клиента.

Задолженность будет отнесена на соглашение с клиентом или на реализацию в зависимости от выбранного порядка расчета.

[![3][3]][3]

Оформление [корректировки реализации товаров](../CRM/CustomerService/FormationOfShipments/FormationOfTheAccompanyingDocuments/AdjustingProductImplementations/AdjustingProductImplementations.md) меняет сумму задолженности клиента. Задолженность может как увеличиться, так и уменьшиться:

[![4][4]][4]

[Возврат товаров от клиента](../CRM/CustomerService/FormationOfAFeedback/ReturnOfProductsFromTheCustomer.md) уменьшает сумму задолженности клиента:

[![5][5]][5]

[1]: FormationOfDebts.assets/1.png
[2]: FormationOfDebts.assets/2.png
[3]: FormationOfDebts.assets/3.png
[4]: FormationOfDebts.assets/4.png
[5]: FormationOfDebts.assets/5.png
