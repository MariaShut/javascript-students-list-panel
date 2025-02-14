### Цель задачи
Практика проверки и преобразования различных видов данных.

### Требования
Создать панель управления студентами, на которой будет располагаться:
- таблица со студентами с фильтрами и сортировкой,
- форма добавления нового студента.


Студенты должны храниться в массиве. Каждый студент — объект, содержащий следующие данные: имя, фамилия, отчество, дата рождения (объект Date), год начала обучения, факультет.


Для добавления студентов на странице должна выводиться форма с полями, соответствующими данным студента. Форма должна проходить валидацию по следующим правилам:
* все поля обязательны для заполнения после применения к значению метода trim();
* дата рождения находится в диапазоне от 01.01.1900 до текущей даты;
* год начала обучения находится в диапазоне от 2000-го до текущего года.


Валидация должна происходить после нажатия на кнопку «Добавить студента», расположенную под полями для ввода. Если валидация прошла успешно, то все поля очищаются, а новый студент добавляется в таблицу. В противном случае под кнопкой выводятся сообщения с описанием ошибок для пользователя.


Данные из массива должны выводиться в табличном виде. Каждая строка таблицы содержит информацию об одном студенте. Колонки таблицы:
* Ф. И. О. студента.
* Факультет.
* Дата рождения и возраст в формате «31.12.2000 (20 лет)». Возраст должен быть вычислен из даты рождения.
* Годы обучения и номер курса в формате «2019-2023 (2 курс)». Считается, что все студенты учатся четыре года, то есть диапазон с годами обучения выводится как {год начала обучения}-{+4 года}. Если сентябрь года окончания обучения уже прошёл, в скобках вместо указания курса должно выводиться «закончил».


Первая строка таблицы — заголовочная, в ней указываются заголовки колонок (Ф. И. О., факультет, дата рождения и возраст, годы обучения). При нажатии на ячейку заголовочной строки должна происходить сортировка по соответствующим полям студентов:
* Ф. И. О. сортирует по соединённой строке из фамилии, имени и отчества по алфавиту по возрастанию.
* Факультет — по факультету по алфавиту по возрастанию.
* Дата рождения и возраст — по дате рождения по возрастанию.
* Годы обучения — по году начала обучения.


Перед таблицей также нужно вывести фильтры, состоящие из полей:
* Ф. И. О. для поиска подстроки в фамилии, имени или отчестве.
* Факультет для поиска подстроки в названии факультета.
* Год начала обучения (точное совпадение).
* Год окончания обучения (точное совпадение).

При любых изменениях в полях для фильтрации содержимое таблицы должно измениться в соответствии с указанными фильтрами. Если указано несколько фильтров, то все они применяются к массиву студентов по очереди.



Реализованы сортировка, фильтрация и добавление элемента в массив к перерисовке таблицы. Таблица всегда содержит актуальные данные.
