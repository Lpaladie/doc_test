# Создание производственного задания на посол мясного сырья

Для создания производственного задания на посол сырья в системе создаются документы **"Производственное задание"**.

- В подсистеме **"Производство"** открываем **"Производственные задания"**:

![](CreateTaskForASalting.assets/1.png)

- Нажимаем на кнопку **"Создать"**:

![](CreateTaskForASalting.assets/2.png)

Заполняем сведения на вкладке **"Основное"**:

1. Дата смены;
2. Смена;
3. Рабочий центр, на котором будет производиться маринование;
  
Поле **"Склад получатель"** не является обязательным для заполнения.
  
Если для разных строк  производственного задания предполагается перемещение выходного изделия на разные склады, следует установить флаг "Указывать склад получатель в таблице".

*В настройках кнопки учетной точки может быть установлен определенный склад получатель по умолчанию. В этом случае склад-получатель при выпуске будет указан по умолчанию из кнопки учетной точки.*

![](CreateTaskForASalting.assets/3.png)

- Заполняем сведения на вкладке **"Задание"**:

  1. Нажимаем на кнопку **"Добавить"** и добавляем нужную номенклатуру в табличную часть;
  2. Заполняем поле **"Характеристика"**, выбрав из списка "Посол";
  3. Спецификация для маринования будет указана автоматически. Если спецификация не появилась в соответствующем поле, значит в системе существует несколько действующих ресурсных спецификаций для производства данного продукта, либо нет ни одной. В этом случае спецификацию необходимо выбрать, открыв список, назначить действующей существующую, или создать новую.
  4. Поле **"Количество"** будет заполнено по спецификации;

Поле **"Партия"** можно заполнить или оставить пустым и тогда партия будет создана автоматически.

- Нажимаем на кнопку **"Провести и закрыть"**.

![](CreateTaskForASalting.assets/4.png)
