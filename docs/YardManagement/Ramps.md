# Рампы

Для хранения списка рамп на складах используется справочник **"Рампы"**, который расположен в разделе **"Склад и доставка"** в подсистеме **"Управление двором"**

[![1][1]][1]

При создании рамп указываются:

- Наименование - используется для представления объекта в системе
- [Склад](../CommonInformation/Warehouse.md)
- Порядок - от порядка зависит какую рампу займет машина, в приоритете находятся рампы с меньшим порядком
- Список [товарных категорий](../CommonInformation/РroductCategory.md) - если список пустой, то с рампы отгружаются все товарные категории. Если список заполнен товарными категориями, то при подборе рампы для машины, в которую должны быть погружены товары указанных товарных категорий, система подберет рампу с наименьшим порядком содержащую одну из категорий из планов отгрузки

[![2][2]][2]

[1]: Ramps.assets/1.png
[2]: Ramps.assets/2.png