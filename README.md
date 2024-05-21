### Owerview

Данное тестовое задание состоит из 3 блоков. Ниже даны постановки задач. Ход решения с комментариями и результаты работы отржаны в ноутбуке [DmitriyAtamanov-25032024-SberIndustry-notebook.ipynb](DmitriyAtamanov-25032024-SberIndustry-notebook.ipynb)

### 1. Python

Написать на python генератор первых n чисел фибоначи.

**Сигнатура:**

```python
def fibonacci_generator(n)
```

**Пример использования:** 

```python
n = 10
for num in fibonacci_generator(n):
    print(num)
```

### 2. Написать Sql-запросы

1. Вывести отдел с наибольшим числом сотрудников;
2. Вывести список сотрудников, получающих заработную плату выше, чем у руководителя;

**Department**

|**Id**|**name**|
| :- | :- |
|1|Финансы|
|2|Риски|
|3|Розница|
|4|Безопасность|
|..|..|
|1000|ДКК|



**Personal**

**id\_head – id – руководителя
id\_dep – id департамента**

|Id|Id\_head|Id\_dep|name|sal|
| :- | :- | :- | :- | :- |
|1|1|2|Бегинс|45 000|
|2|1|2|Поттер|80 000|
|3|2|2|Чапаев|100 000|
|4|4|4|Шилов|65 000|
|…|..|..|..|..|
|10000|5|3|Наумов|64 500|



### 3. Задачка на определение отрасли компании

**Таблица Pays** - платежи между компаниями

|***hash\_inn\_kt***|Обезличенный ИНН отправителя|
| :- | :- |
|***hash\_inn\_dt***|Обезличенный ИНН получателя|
|***week***|Неделя|
|***count***|Кол-во платежей в неделю|
|***sum***|Сумма платежей в неделю; (обезличенная)|

**Таблица inn\_info\_public** - Информация по компаниям

|***hash\_inn***|Обезличенный ИНН|
| :- | :- |
|***okved2***|Обезличенная отрасль |
|***region***|Обезличенный регион |
|***is\_public***|Флаг выборка для обучения \ контрольная|



В задаче необходимо для компаний с флагом -1 в поле okved2 файла inn\_info\_public проставить их отрасль. (Задача много-классовой классификации)