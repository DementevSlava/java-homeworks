## Задача 3. База организаций
### Описание
Вы разрабатываете государственную систему учета организаций. Организация представлена следующими атрибутами – Название, город, адрес, ИНН, КПП, ОГРН. Ключом уникальности организации является сочетание “ИНН”+”КПП”+”ОГРН”.
Пользователь вводит организации, аналогично заданию “Список сотрудников”.
Структура данных, куда сохраняются организации должна отбрасывать ввод одной и той же организации 2 раза.

### Реализация
1. Создайте класс `Organization` с полями `Name`, `City`, `Address`, `INN`, `KPP`, `OGRN`. Тип всех полей – `String`.
2. Переопределите методы hashcode и equals для класса `Organization` так, чтобы нельзя было сохранить двух организаций, у которых все три поля: "ИНН", "КПП", "ОГРН" были бы одинаковыми.
3. Продемонстрируйте добавление объектов класса в HashSet, ошибку при добавлении организаций с тремя одинаковыми параметрами, возможность существования нескольких организаций с одинаковым названием, городом и адресом.