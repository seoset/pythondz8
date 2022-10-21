Задача создать информационную систему позволяющую работать с сотрудниками некой компании \ студентами вуза \ учениками школы

Порядок работы информационной системы:

Программа генерирует (или уже имеет) готовый файл school_list который содержит например ID, ФИО, ДР, успеваемость, пол ученика. Пользователю предлагается на выбор отсортировать данные в файле, далее программа выводит результат на экран.

Структура информационной системы:

1.	модуль Processing_Data
функции
def append_info
def delete_info
(+ функция генерации)
возвращает обработанный список

2.	модуль Editor_file
функции
def read_file
def write_file
def create_test_file
def save_file
•	Считывает инф из БД
•	Кладет в переменную
•	Получает список для сохраненя

3.	модуль Processing_file def
•	Получает данные (выбор юзера)
•	Получаете исходный список
•	Формирует необходимый список
•	возвращает список

4.	модуль Print_List функция
def console_print
•	Получает список
•	Выводит его на консоль
•	возвращает список

5.	модуль User_Interface
функция
def user_choice
Обращается к пользователю для выбора режима
•	Вывод всей информации
•	Вывод всех ДР
•	Вывод успеваемости
•	Вывод пола

6.	модуль ТГ Бота
активирует Телеграм-Бота для управления информационной системой
(запросы пользователя и результаты выводятся в мессенджере)

