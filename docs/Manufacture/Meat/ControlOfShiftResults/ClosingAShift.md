# Рабочее место мастера смены

Для контроля результатов производства за смену  в системе существует специальное рабочее место.

- В подсистеме **"Производство"** открываем **"Рабочее место мастера смены"**:

![](ClosingAShift.assets/1.png)

По гиперссылке **"Настройки смены"** открываем окно для ввода параметров смены.

- Вводим дату смены  вручную. Смена и временной диапазон заполнятся автоматически, при необходимости их можно скорректировать вручную.

![](ClosingAShift.assets/2.png)

- Закрываем окно ввода параметров смены и выбираем рабочий участок, на котором необходимо подвести итоги смены.

  Нажимаем кнопку "Обновить", в табличной части ниже появится информация о рабочем участке и рабочих центрах, закрепленных за ним.  Выбираем нужный вид рабочего центра, а затем рабочий центр:

![](ClosingAShift.assets/3.png)

# Задания

- На вкладке **"Задания"** можно увидеть информацию о выпущенных продуктах за текущую смену.

  Чтобы создать задание на смену, нажимаем на кнопку **"Создать задание"** в шапке вкладки. Откроется стандартная форма документа **"Производственное задание"**;

![](ClosingAShift.assets/4.png)

В табличной  части указана номенклатура произведенных продуктов, количество, которое планировалось произвести, фактически произведенное количество и процент отклонения от плана.

Возможны ситуации, когда физически произведено одно количество продукта, а по документам в системе указано другое. Если причиной отклонения является ввод ошибочных данных сотрудником цеха, созданные документы можно скорректировать.

Для этого выбираем партию, нажимаем кнопку **"Корректировка"** и выбираем пункт выпадающего списка **"Откорректировать количество"**:

![](ClosingAShift.assets/5.png)

В открывшемся окне вводим новое значение количества выпущенной продукции в используемых единицах измерения (кг, шт.)

- Нажимаем на кнопку **"ОК"**:
  
![](ClosingAShift.assets/6.png)
  
Откроется окно корректировки документов. Следует ознакомиться со списком и содержанием документов  и отметить флагом те, которые необходимо изменить.

- По завершении проверки нажимаем на кнопку **"ОК"**:
  
![](ClosingAShift.assets/7.png)
  
- В основном окне рабочего места появится следующее сообщение:

![](ClosingAShift.assets/8.png)

# Остатки
  
- На вкладке **"Остатки"** отображаются текущие остатки материалов на складах рабочего центра и обороты сырья за смену.

  Если за текущую смену физически были зафиксированы потери по материалу, а в системе числятся остатки на складе, следует списать остатки с отнесением на потери при производстве. Для этого разворачиваем вкладку действий:
  
![](ClosingAShift.assets/9.png)
  
- Нажимаем на кнопку **"Списать"**:

![](ClosingAShift.assets/10.png)

Открылось окно списания. Выбираем вариант списания и нажимаем **"ОК"**:

![](ClosingAShift.assets/11.png)

В таблице ниже автоматически скорректируется количество прихода и расхода по выбранной номенклатуре:

![](ClosingAShift.assets/12.png)

# Закрытие рабочей смены

- Когда  мастер смены удостоверился, что за текущую смену в систему введена корректная информация о выходах и остатках, следует закрыть смену на рабочем центре.

Переходим к закладке **"Закрытие смены"** и нажимаем кнопку **"Закрыть смену"**. 

![](ClosingAShift.assets/13.png)

- Откроется предупреждение о закрытии смены по рабочим центрам:

![](ClosingAShift.assets/14.png)

Если при закрытии смены система выявит некорректные данные, статус смены в табличной части слева изменится на **"Есть ошибки"**, а на закладке **"Закрытие смены**" отобразится информация о некорректных данных.

- Если все данные за смену верны, статус смены на рабочем центре изменится на **"Закрыта"**:

![](ClosingAShift.assets/15.png)