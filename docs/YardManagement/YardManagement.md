# Управление двором

АРМ **"Управление двором"** используется для управления статусами *Заданий на доставку* и подбора рамп, он расположен в разделе **"Склад и доставка"** в подсистеме **"Управление двором"**

[![1][1]][1]

После открытия АРМа заполняются [настройки](YardManagementSettings.md)

[![2][2]][2]

[![3][3]][3]

Дата отгрузки заполняется из настроек, при желании можно изменить ее вручную.

В верхней части формы отражаются все доступные статусы заданий на доставку из настройки. При переключении на статус выводится список заданий на доставку в этом статусе. Так же возможен вариант, что будут выводиться задания на доставку в предыдущем статусе, если этот статус был добавлен в настройках в пропускаемые.

В АРМе **"Управление двором"** могут отражаться статусы начиная с **"К погрузке"** и заканчивая **"Оформлено"** (статусы Формируется, Погружено, Отправлено и Закрыто не отражаются).

При изменении статуса от **"К погрузке"** к **"Ожидает подготовки"** автоматически подбирается рампа.

В статусе **"Ожидает подготовки"** можно выбрать другую рампу с помощью кнопки **"Изменить рампу"**.

Для каждого статуса есть возможность перевести задание в предыдущий статус с помощью кнопки **"<<"**, либо в следующий с помощью кнопок:

- Для статуса "К погрузке" - **"Впустить на территорию"** - статус сменится на "Ожидает подготовки"
- Для статуса "Ожидает подготовки" - **"Приступить к подготовке"** - статус сменится на "К подготовке"
- Для статуса "К подготовке" - **"Приступить к погрузке"** - статус сменится на "Загружается"
- Для статуса "Загружается" - **"Погрузить"** - статус сменится на "Погружено"

!!! attention ""

    После того как статус задания на доставку станет **Погружено** по нему должны быть сформированы накладные в АРМе **Формирование накладных** и переведены в статус **Выдана**, тогда статус задания на доставку сменится на **Оформлено** и с ним можно будет работать дальше в управлении двором

- Для статуса "Оформлено" - **"Выпустить с территории"** - статус сменится на "Отправлено"

[![4][4]][4]

[1]: YardManagement.assets/1.png
[2]: YardManagement.assets/2.png
[3]: YardManagement.assets/3.png
[4]: YardManagement.assets/4.png
