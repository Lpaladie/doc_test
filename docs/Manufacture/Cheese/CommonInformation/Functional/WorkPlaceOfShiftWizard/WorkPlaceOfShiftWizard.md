**Действия в Рабочем месте мастера смены**
==========================================

В рабочем месте мастера смены присутствует довольно много операций, что
объясняется вовлечением мастера смены во все процессы цеха. Потому и
было решено все эти действия объединить в одном месте.

<h2> Вкладка "Выпуск" </h2>

![](WorkPlaceOfShiftWizard.assets/drex_dejstviya_v_rabochem_meste_mastera_smeny_custom_9.png)

<h3> Задание </h3>

открывает ранее созданный документ "Производственное задание" на указанную смену на выбранный РЦ или же открывает форму создания задания на эту смену.

<h3> Корректировка </h3>

![image-20200818085824546](WorkPlaceOfShiftWizard.assets/image-20200818085824546.png)

- Количество: позволяет внести правки в количество выпуска по выбранной партии в таблице "Выпуск";
- Номенклатура: позволяет изменить вид продукции у выбранной в таблице "Выпуск" партии

<h3> Перераспределить сырье </h3>

В случае, если за смену были выпуски побочной продукции, на которую обычно не списывается основной ингредиент (Сыворотка, Обрат и тп), а на основные выпуски списание идет, этой кнопкой делается "минус" по расходу на основные выпуски и "плюс" по расходу на вторичные выпуски.  
Распределение требует учтенных в системе показателей жира и белка по каждой партии выпуска и каждой партии основных материалов, т.к. разделение идет именно на основании этих показателей.

<h2> Вкладка "Остатки" </h2>

![](WorkPlaceOfShiftWizard.assets/drex_dejstviya_v_rabochem_meste_mastera_smeny_custom.png)

На текущей вкладке можно смотреть приход/расход/остатки по полуфабрикатам, продукции и материалам и сырью.

При этом, выбрав "Диаграмма", можно смотреть только остатки, однако, в более наглядной форме. Такое обычно удобнее для участков, где происходит переработка "жидких" материалов.

<h3> Списать усушку </h3>

требует наличие расхода и конечного остатка.  
Это действие можно сделать:  
​1) для одной серии (выделив только её)  
​2) для нескольких серий (выделив несколько)  
​3) сразу для всего склада (просто выделив склад в таблице).  
Предполагает списывать остатки в бассейне\\на обсушке\\в камерах
созревания. Когда на входе было одно количество сыра, на выходе
получилось чуть меньше (по кг - сыр усыхает).  

1. Выбрать партию (партии, склад) - нажать "Списать усушку".   
![](WorkPlaceOfShiftWizard.assets/drex_dejstviya_v_rabochem_meste_mastera_smeny_custom_2.png)  
2. Создается документ "Распределение материалов". Распределение идет один в один (на что серия сыра тратилась, на ту партию усушка и списывается).

<h3> Объединить партии </h3>

позволяет объединить несколько серий одной продукции в одну.  
Применяется при выпуске производственной партии молока. На входе есть много партий от разных поставщиков, на выходе - одна партия (накопился танк сырого молока - берется контрольный анализ, и молоко переходит в производственную партию).

1. Выбрать партию (партии, склад) - нажать "Объединить партии",
    подтвердить количество выхода (автоматически - сумма всех выделенных
    партий).  
![](WorkPlaceOfShiftWizard.assets/drex_dejstviya_v_rabochem_meste_mastera_smeny_custom_3.png)  
2. Создается документ "Переработка", где в выпуске молоко с новой
    партией, а в материалах - все партии, которые были выделены (или все
    серии в танке, если позиционирование было на складе и если там была
    одна номенклатура).

??? Info "В режиме диаграммы объединяются все партии склада, независимо от количества выделенных"

<h3> Указать выпуск </h3>

позволяет указать на какой-либо из складов РЦ выпуск.   
Предполагает учет выпусков сливок, смеси, обрата и других полуфабрикатов приемно-аппаратного цеха.

1. Выбрать в таблице склад выпуска - нажать "Указать выпуск". Указать,
    что и в каком количестве выпускается. При этом можно выбрать один из
    трех вариантов списания материалов (не распределять, по норме -
    указывается склад (склады), с которого берется основной материал (по
    спецификации), целиком по спецификации - все остатки (по рецептуре) на указанном складе (складах)
    будут списаны на этот выпуск).  
![](WorkPlaceOfShiftWizard.assets/drex_dejstviya_v_rabochem_meste_mastera_smeny_custom_4.png)  
2. При этом, если выпускаемая продукция имеет одну единицу измерения, то количество можно получить, как сумму всех материалов по основной спецификации, чья единица измерения совпадает с единицей измерения выпуска.  
![](WorkPlaceOfShiftWizard.assets/drex_dejstviya_v_rabochem_meste_mastera_smeny_custom_11.png)  
3. Создается документ "Переработка", где в выпуске указанная
    номенклатура и количество, материалы заполняются по указанному
    правилу.

<h3> Переместить </h3>

позволяет перемещать партии продукции между складами.  
Предполагает учет передач сливок, обрата в другие цеха или склады цеха.

1. Выбрать в таблице партию (партии) - нажать "Переместить". Указать
    куда и сколько перемещается.  
![](WorkPlaceOfShiftWizard.assets/drex_dejstviya_v_rabochem_meste_mastera_smeny_custom_5.png)  
2. Создается документ "Распоряжение на перемещение".

<h3> Списать </h3>

формируется документ "Распределение материалов".  

- **Согласно спецификации** - требует наличие выпуска по
    спецификации, где выбранный остаток конфигурирует, как материал.
    Списание идет на все выпуски, по которым выбранный остаток мог бы
    быть потрачен.  
    Например, есть пакет красный. С его использованием упаковывают
    несколько варок сыра "Российский 3\\19", "Пошехонский 5\\19". В
    каждой спецификации этот пакет указан в материалах. При
    распределении этот пакет списывается и на Российский, и на
    Пошехонский.  
    -   Выбрать материал (и серию) - нажать "Списать". Указать вариант
    списания "Согласно спецификации" и указать списываемое количество.

- **Пропорционально списанному** - требует наличие выпуска, где
    материал, по которому есть остаток, уже был потрачен.
    Например, так же пакеты красные. Потратились на упаковке на сыр
    "Российский" и на сыр "Пошехонский". Но при этом, на пошехонский сыр
    не стоит в спецификации. В варианте **a.** пакеты списались бы
    только на российский сыр, а в текущем - на оба. 
    -   Выбрать материал (и серию) - нажать "Списать". Указать вариант
    списания "Пропорционально списанному".

- **По отраслевой методике** - не требует расхода материала, но
    требует наличие выпусков, на которые этот материал может быть
    потрачен. Также требует наличия анализов по жиру и белку.  
    Списывается на все выпуски, пропорционально содержанию жира и белка
    в них.  
    Например, применяется на переделе, когда есть выпуски смесей, сливки
    и обрат. Все молоко списывают на все выпуски согласно содержанию
    жира и белка в них.  
    -   Выбрать партию молока - нажать "Списать". Указать вариант списания
    "По отраслевой методике" и указать количество.

- **Брак**- требует расхода материала. В текущем функционале виден
    только для номенклатуры с типом "Короб" или "Пакет".  
    Предполагает списание бракованных коробов или пакетов, выявленных в
    процессе их использования за смену. Указанный материал списывается
    со статьей брака на уже имеющиеся выпуски пропорционально
    потраченному.
    -   Выбрать короб или пакет (и серию) - нажать "Списать". Указать
    вариант списания "Брак", указать количество и статью затрат для
    брака.

    ![image-20200818091735836](WorkPlaceOfShiftWizard.assets/image-20200818091735836.png)

<h3> Заменить материал </h3>

требует наличие расхода заменяемого материала. Указанное количество заменяемого материала приходуется, а чем заменяем – расходуется на ту продукцию, на которую тратился заменяемый.  
1. Перейти на вкладку "Остатки" -\> "Материалы" (или "Прочее"), найти
    заменяемый материал (и его серию) - нажать "Заменить материал".
    Указать, чем заменяется (и серию), количество для замены.  
![image-20200818090413350](WorkPlaceOfShiftWizard.assets/image-20200818090413350.png)
2. Формируется документ "Распределение материалов".