# Установка шаблонов идентификаторов партий продукции в Меркурии

Чтобы в Меркурий партии приходили с понятными идентификаторами, можно задать для каждой продукции шаблон, по которому они будет формироваться. При этом можно задать шаблон на уровне вида продукции, а можно переопределить его на уровне продукции.

## Шаблон для вида продукции

- Открыть справочник "Виды продукции" (можно открыть из Наименования продукции)

- Открыть нужный вид:

  ![1](TemplatesOfID.assets/1.png)

  ![2](TemplatesOfID.assets/2.png)

- Перейти по ссылке "Шаблоны идентификаторов партий ГИСМ":

  ![3](TemplatesOfID.assets/3.png)

- Нажать "Создать". После этого появится окно, в нем нажать кнопку редактирования:

  ![4](TemplatesOfID.assets/4.png)

- Создать шаблон, используя данные, представленные таблице слева, и операторы, представленные в таблице справа:

  ![5](TemplatesOfID.assets/5.png){: width=70%}

- поле формулы ввести новую. Например, при использовании такой формулы: 

`Прав(Формат([ДатаВыработки] , "ДФ='dd.MM.yy'"),2) + Лев(Прав(Формат([ДатаВыработки] , "ДФ='dd.MM.yy'"),5),2) + Лев(Формат([ДатаВыработки] , "ДФ='dd.MM.yy'"),2) + [НаименованиеПродукции.Артикул]`

наименования партий будут выглядеть так **20070235135135**, где 35135135 - Артикул продукции.

![6](TemplatesOfID.assets/6.png)

- Нажать "Сохранить и закрыть".

- Нажать "Записать и закрыть":

  ![7](TemplatesOfID.assets/7.png)

## Шаблон для продукции

- Открыть справочник "Наименование продукции":

![8](TemplatesOfID.assets/8.png){: width=70%}

- Открыть нужную продукцию:

![9](TemplatesOfID.assets/9.png){: width=70%}

- Перейти по ссылке "Шаблоны идентификаторов партий ГИСМ":

![10](TemplatesOfID.assets/10.png)

- В открывшемся окне нажать "Создать". После этого появится окно, в нем нажать кнопку редактирования:

![11](TemplatesOfID.assets/11.png){: width=70%}

- Создать шаблон, используя данные, представленные таблице слева, и операторы, представленные в таблице справа:

![12](TemplatesOfID.assets/12.png){: width=70%}

- В поле формулы ввести новую. Например, при использовании такой формулы: 

`Прав(Формат([ДатаВыработки] , "ДФ='dd.MM.yy'"),2) + Лев(Прав(Формат([ДатаВыработки] , "ДФ='dd.MM.yy'"),5),2) + Лев(Формат([ДатаВыработки] , "ДФ='dd.MM.yy'"),2) + [НаименованиеПродукции.Артикул]`

наименования партий будут выглядеть так **20070235135135**, где 35135135 - Артикул продукции.

![13](TemplatesOfID.assets/13.png)

- Нажать "Сохранить и закрыть".
- Нажать "Записать и закрыть":

![14](TemplatesOfID.assets/14.png)