# Распределение затрат

Документы **"Распределение затрат"** предназначены для распределения затрат по аналитикам отгруженной продукции. Распределение используется для формирования финансового результата.

Документы **"Распределение затрат"** расположены в разделе **"Деньги"** в подсистеме **"Закрытие месяца"**:

[![2][2]][2]

В документе можно указать [сценарий](CostAllocationScenario.md), остальные поля документа будут заполнены по нему автоматически. Кнопка **"Заполнить и распределить"** позволяет выполнить заполнение таблиц **"Затраты"**, **"База"** и распределить затраты в соответсвии с выбранным сценарием одним действием.

Если сценария нет, то заполняются поля:

- [Организация](../CommonInformation/Organization.md)
- [Направление деятельности](DirectionOfActivity.md)

На вкладке **"Затраты"** заполняются отборы:

- По дате: либо устанавливается признак **"На конец месяца"**, тогда затраты будут заполняться на конец месяца, либо заполняется поле **"На"** - элемент справочника **Варианты начала периода**, который отвечает за дату на которую расчитываются затраты

[![5][5]][5]

- [Подразделение](../CommonInformation/Department.md) - отвечает за то по каким подразделениям будут выбираться затраты
- [Статья затрат](ItemsOfExpenditure.md) - отвечает за отбор затрат по указанным статьям
- Аналитика затрат - отвечает за отбор затрат по указанным аналитикам
- Отбор - позволяет установить дополнительные отборы
- Сортировка - позволяет задать порядок затрат

[![6][6]][6]

Далее по кнопке **"Заполнить"** табличная часть заполняется затратами согласно установленным отборам, заполняются поля:

- [Подразделение](../CommonInformation/Department.md)
- [Статья затрат](ItemsOfExpenditure.md)
- Аналитика затрат
- Сумма

[![1][1]][1]

На вкладке **"База"** заполняются отборы:

- По дате: либо устанавливается признак **Месяц документа**, тогда база определяется за весь месяц в который создано распределение затрат, либо устанавливается период расчета базы

[![7][7]][7]

- Признак **"База на каждую строку затрат"** - устанавливается для того, чтобы для каждой строки затрат определялась своя база
- В таблице устанавливаются отборы по которым определяется база (например, если распределяются затраты на доставку нам сторонней транспортной компанией, то базу нужно расчитывать по Перевозчику):

    - Торговый представитель - менеджер [точки доставки](../CommonInformation/DeliveryPoint.md)
    - Менеджер направления - менеджер группы партнеров для планирования
    - Менеджер клиента - менеджер [контрагента](../CommonInformation/Contractor.md)
    - [Товарная категория](../CommonInformation/РroductCategory.md)
    - Маркетинговое мероприятие
    - [Перевозчик](../CommonInformation/Contractor.md)
    - Транспортное средство
    - Водитель
    - [Задание на доставку](../CRM/CustomerService/FormationOfShipments/PlanningOfShipments/DistributionOfShipmentsByCar.md)
    - [Холдинг](../CommonInformation/Holding.md)
    - [Контрагент](../CommonInformation/Contractor.md)
    - [Заказ клиента](../CRM/CustomerService/FormationOfOrders/CustomerOrder.md)
    - [Подразделение](../CommonInformation/Department.md)
    - Отбор - позволяет установить дополнительные отборы
    - Сортировка - позволяет задать порядок базы

[![8][8]][8]

По кнопке **"Заполнить"** табличная часть вкладки заполняется отгрузками по установленным отборам согласно аналитикам затрат, заполняются поля:

- [Номенклатура](../CommonInformation/Nomenclature.md)
- [Контрагент](../CommonInformation/Contractor.md)
- [Заказ клиента](../CRM/CustomerService/FormationOfOrders/CustomerOrder.md)
- [Документ продаж](../CRM/CustomerService/FormationOfShipments/ProductsShipment.md)
- [Подразделение](../CommonInformation/Department.md)
- Количество
- Сумма
- Вес
- Себестоимость
- Валовая прибыль

[![3][3]][3]

На вкладке **"Расходы"** заполняются:

- Показатель:

    - Количество - затраты будут распределяться пропорционально количеству отгружаемого товара
    - Сумма - затраты будут распределяться пропорционально сумме за отгружаемый товар
    - Вес - затраты будут распределяться пропорционально весам отгружаемого товара
    - Себестоимость - затраты будут распределяться пропорционально себестоимости отгружаемого товара
    - Валовая прибыль - затраты будут распределяться пропорционально валовой прибыли от отгружаемого товара

- Пояснение - произвольный комментарий

По кнопке **"Распределить"** на вкладке табличная часть заполняется распределенными по базе затратами, заполняются поля:

- [Подразделение](../CommonInformation/Department.md)
- [Контрагент](../CommonInformation/Contractor.md)
- [Заказ клиента](../CRM/CustomerService/FormationOfOrders/CustomerOrder.md)
- [Номенклатура](../CommonInformation/Nomenclature.md)
- [Статья затрат](ItemsOfExpenditure.md)
- Аналитика затрат
- Показатель
- Сумма

[![4][4]][4]

[1]: CostAllocation.assets/1.png
[2]: CostAllocation.assets/2.png
[3]: CostAllocation.assets/3.png
[4]: CostAllocation.assets/4.png
[5]: CostAllocation.assets/5.png
[6]: CostAllocation.assets/6.png
[7]: CostAllocation.assets/7.png
[8]: CostAllocation.assets/8.png
