# Настройка обмена по расписанию

Регламентный обмен нужен для регулярного фонового получения необходимой информации через автоматизированную отправку запросов.

[![1][1]][1]

[![2][2]][2]

Можно настроить командой из справочника записей журнала или из списка ВСД.

Признак *"частое"* отвечает за то, какое конкретно задание будет выполняться. Частое захватывает еще и классификаторы.

- Частое – раз в час
- Не частое – раз в день

Виды бизнес операций:

- **Список ВСД** - грузит ВСД (возможно настроить по отборам) по периоду
- **История ВСД** - актуализирует/добавляет ВСД, измененные за период
- **Записи журнала** - грузит список неотправленных записей журнала (с положительным остатком)
- **История журнала** - грузит записи журнала, изменённые за период

**Сдвиг начала периода** – если предыдущий регламент отработал 10 числа, а следующий выполняется 15, то при сдвиге равном 0 будет получена история с 10 по 15. Если сдвиг равен 7, то будет получена история с 3 по 15.

Сдвиг обеспечивает нахлест получения истории, чтобы не пропустить объекты, которые были изменены в пограничное время.

Если сдвиг большой (7 дней, например) то будут получены данные за 7 дней, которые уже были получены ранее, они будут распарсены и по этим данным проактуализированы объекты. Если синхронизация выполняется каждый час, то сдвиг в 7 дней будет тупо нагружать систему бесполезными данными. Рекомендуется ставить либо 0.5 для редких заданий, либо 0.1 для частых.

**Частота запроса** – Частое/Не частое. Есть 2 регламентных задания по актуализации - частое и обычное. Частое по умолчанию настроено на раз в час, обычное - раз в день. Этот флаг определяет на какое регламентное задание упадет этот обмен, но расписания могут быть изменены в том числе на противоположные - обычное регламентное задание раз в час, а частое - раз в месяц.

**Инициатор** – пользователь ГИС Меркурий, под которым будут уходить запросы в ГИС Меркурий.

Более детально расписание регламентных заданий можно настроить стандартной обработкой **регламентные и фоновые задания**.

[![3][3]][3]

[1]: SettingScheduledExchange.assets/1.png
[2]: SettingScheduledExchange.assets/2.png
[3]: SettingScheduledExchange.assets/3.png
