# __2 Обоснование метода организации входной и выходной информации__ #


Информационное обеспечение — это совокупность единой системы
классификации и кодирования информации, унифицированных систем
документации, схем информационных потоков, циркулирующих в организации, а
также методология построения БД.
База данных включает в себя 6 сущностей.
Таблица «Владельцы» содержит список владельцев ТС в данном ДТП.
Первичным ключом является поле код владельцы. Ключевые атрибуты сущности
представлены в таблице 1.

Таблица 1 - "Владельцы"
| Имя поля | Тип данных | Особенности
|--------|-------|------|
|Код_владельца|int|Первичный ключ|
|Фамилия|varchar(30)|not null|
|Имя|varchar(30)|not null|
|Отчество|varchar(30)|not null|
|Паспортные данные|varchar(30)|not null|
|Полис ОСАГО|varchar(30)|not null|
|Адрес|varchar(30)|not null|
|Страховая компания|int|not null|
Таблица «Транспортные средства» содержит информацию о транспортных
средствах. Первичным ключом является поле код транспортного средства.
Ключевые атрибуты сущности представлен в таблице 2.

Таблица 2 - "Транспортные средства"
| Имя поля | Тип данных | Особенности
|--------|-------|------|
|Код_тс|int|Первичный ключ|
|Госномер|int|not null|
|Категория|varchar(30)|not null|
|Марка|varchar(30)|not null|
|Модель|varchar(30)|not null|
|Цвет|varchar(30)|not null|
|Год выпуска|date|not null|
|Дата регистрации|date|not null|

# 3 Функционирование программы #


Программа «Учёт ДТП» написана на языке C#, c использованием SQL Server
в качестве хранения данных и с приложением Visual Studio. [7]
В системе присутствует модуль «Авторизации»(AutorizationWindow.xaml), с
помощью которого выполняются команды по авторизации пользователя в системе с
проверкой логина и пароля. (См. Рисунок 1)

![Logo Image](https://www.joomfox.org/images/blog/review/3838/01.png "Окно авторизации")
Рисунок 1 - окно авторизации.

Таким образом, можно выделить следующие основные преимущества
использования автоматизированной информационной системы на основе
вычислительной техники для решения задачи построения системы учета:
+ Повышение удобства поиска и отбора данных из справочников хранения
статической информации и журналов выполненных операций,
+ повышение скорости поиска и отбора информации, а также оформления
операций с недвижимостью,
+ обеспечение влияния каждых вновь появившихся предложений на рынке
недвижимости на старые заявки клиентов,
+ обеспечение безопасности хранения информации,
+ обеспечение многопользовательской работы.
