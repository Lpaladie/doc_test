# АРМ ветеринарного врача

Автоматизированное рабочее место ветеринарного врача предназначено для создания и отправки заявок в ГИС Меркурий. Заявки на операции автоматизировано заполняются на основании документов оперативного учёта, соответствий справочников и правил формирования партий.

В шапке АРМа вет. врача указываются:

- [Сценарий заполнения партий](WorkplaceScenarios.md) – сохраненные параметры для заполнения партий
- Период – для отбора документов оперативного контура
- Предприятие – основная площадка
- Значения – параметры для заполнения партий, если не задан сценарий

[![1][1]][1]

В правой части, через пункт меню **"Ещё"**, можно перейти ко всем связанным настройкам формирования партий.

[![2][2]][2]

У рабочего места ветеринарного врача следующие вкладки:

- [Производство](Production.md) – вкладка на которой происходит создание производственных партий на основании данных оперативного учета
- [Обеспечение](Provision.md) – вкладка для формирования транспортных ВСД на основании документов задание на доставку, реализация товаров и услуг и перемещение товаров

В нижней части АРМа отображён список ВСД. Можно отключить командой **"Показать ВСД"** ВСД можно отобрать по связанному документу. Связанный документ активизируется в закладках выше.

[![3][3]][3]

[1]: WorkplaceVeterinarian.assets/1.png
[2]: WorkplaceVeterinarian.assets/2.png
[3]: WorkplaceVeterinarian.assets/3.png
