# Отгрузка товаров

Отгрузка товаров относится к системе складской логистики. Рассмотрим вариант отгрузки с неавтоматизированного склада.

Для возможности работы с неавтоматизированными складами нужно в **"Настройках исполнения заказов"** установить флаг **"Использовать неавтоматизированные склады при оформлении накладных"**.

[![1][1]][1]

[![2][2]][2]

Для пользователей, которые занимаются созданием распоряжений на отгрузку и накладных для неавтоматизированных складов в системе создан поставляемый профиль доступа *"Формирование накладных на неавтоматизированных складах"*.

[![3][3]][3]

Для формирования **"Распоряжений на отгрузку"** на неавтоматизированном складе используется вкладка **"Формирование распоряжений"** обработки **"Формирование накладных"**, которая расположена в разделе **"Заказы"** в подсистеме **"Обработка заказов клиентов"**.

[![4][4]][4]

После открытия обработки заполняем:

- Период
- Склад - не обязательно заполнять (позволяет делать отгрузки по определенному складу)

Затем нажимаем кнопку **"Обновить"**, в левой части обработки будет выведен список *"Заданий на доставку"*, у которых установлен статус **К погрузке** и планы отгрузок которых находятся в статусах **"Запланировано"**, **"В наборку"** или **Набирается**, плановое количество к отгрузке и фактически набранное количество товаров.

При переходе к планам отгрузки, которые погружены в машину в правой верхней части обработки выводится список товаров планируемых к отгрузке.

В нижней правой части выводится список распоряжений на отгрузку и отгруженных товаров, а так же добавляются товары для отгрузки. Можно заполнить табличную часть с помощью кнопок **"Отгрузить"** или **"План в Факт"**. Там же формируются новые, редактируются уже созданные **"Распоряжения на отгрузку"** после нажатия на кнопку **"Сохранить"**.

Кнопкой **"Отгрузить"** формируются распоряжения на отгрузку по выделенным планам с учетом остатков (используются либо свободные остатки, либо прогнозные остатки производства, если у склада установлен признак "Использовать прогнозный регистр"). Номенклатура из остатков подбирается по разрешенному для контрагента остаточному сроку годности.

Кнопка **"План в Факт"** переносит только номенклатуру, характеристики и количества, без подбора серий, они в дальнейшем заполняются вручную. После редактирования, заполнения таблицы Факт изменения нужно сохранить.

Создадим **"Распоряжение на отгрузку"** по заданию на доставку на 29.05.2020

В АРМе заполняем:

- Период: 01.05.2020 - 31.05.2020
- Склад - Склад готовой продукции

Нажимаем кнопку **"Обновить"**.

[![5][5]][5]

Далее переходим к плану отгрузки, с помощью кнопки **"План в Факт"** заполняем табличную часть отгружаемых товаров, заполняем серии для товаров:

- Сыр Адыгейский - 00001 до 27.02.2020 0:00:00
- Сыр Костромской - 00002 до 27.02.2020 0:00:00
- Сыр Пошехонский - 00003 до 27.02.2020 0:00:00

Нажимаем кнопку **"Сохранить"**, будет создано **"Распоряжение на отгрузку"**.

[![6][6]][6]

Для того, чтобы перевести план отгрузки в статус **"Набирается"** и распечатать для кладовщика список товаров для отгрузки, нажимаем кнопку **"Набрать"**

[![7][7]][7]

[![8][8]][8]

[![9][9]][9]

Переходим к **"Распоряжению на отгрузку"** и проверяем, что оно сформировалось корректно.

[![10][10]][10]

Для отражения завершения работы по отгрузке необходимо в обработке нажать на кнопку **"Подтвердить"**, после этого **"План отгрузки"** будет переведен в статус **Собрано** и не будет отображаться в АРМе.

[![11][11]][11]

[![12][12]][12]

[1]: ProductsShipment.assets/1.png
[2]: ProductsShipment.assets/2.png
[3]: ProductsShipment.assets/3.png
[4]: ProductsShipment.assets/4.png
[5]: ProductsShipment.assets/5.png
[6]: ProductsShipment.assets/6.png
[7]: ProductsShipment.assets/7.png
[8]: ProductsShipment.assets/8.png
[9]: ProductsShipment.assets/9.png
[10]: ProductsShipment.assets/10.png
[11]: ProductsShipment.assets/11.png
[12]: ProductsShipment.assets/12.png