# Производство

На вкладке **"Производство"** есть три основные вкладки:

- Переработка (если доступна лицензия на переработку) - здесь отображены документы переработок на основании которых можно сформировать производственную партию
- Производственные партии – журнал документов производственная партия
- Незавершенное производство – основная закладка для создания производственных транзакций

## Вкладка незавершенное производство

На закладке **Незавершенное производство** отбирается подконтрольная продукция по документам, указанным в [**Перечне документов оперативного учёта НЗП**](../NormativeReferenceInformation/FormationOfParties/ListOfOperationalAccountingDocuments.md).
Для отбора продукции, необходимо указать в параметрах закладки дату выпуска (дата изготовления в справочнике серия). Указать Предприятие производитель и ХС производитель.

Основные команды:

- **Оформить** - создаёт заявку и вызывает групповую форму синхронизации для обмена с ГИС
- **Закрыть** - команда закрытия транзакции

Настройки:

- Открывать партию – открывается форма документа до синхронизации
- Прикреплять лабораторные исследования – вызов автоматизированного прикрепления ветеринарных событий
- Отображать несобранные планы отгрузки – если закладка настроена на реализации товаров, зависит от статуса связанного плана отгрузки. Если признак не установлен, тогда отображается продукция по планам только со статусом собрано.

[![1][1]][1]

Вся продукция группируется по виду продукции (3-й уровень классификации наименований продукции).

Табличная часть вкладки содержит следующие поля:

- Оперативные данные – объем продукции итого за период по движениям документов на дату выпуска из шапки
- Произведено – количество в производственных ВСД
- К производству – разница между опер. данными и произведено. На данное количество создается документ
- Годен до – срок окончания годности
- НЗП – признак незавершенной транзакции. Устанавливается в настройках формирования партий
- Закрыта – признак закрытия транзакции. Не отобразится, если транзакция закрыта в веб интерфейсе
- Подбор сырья – признак оперативного подбора сырья. Устанавливается в настройках формирования партий
- Показать – гиперссылка для перехода в связанные документы.

[![2][2]][2]

[1]: Production.assets/1.png
[2]: Production.assets/2.png
