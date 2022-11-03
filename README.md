# Mindbox_test_cases
Test cases of mindbox company


**Задание №1**

Есть Pandas DataFrame со столбцами [“customer_id”, “product_id”, “timestamp”], который содержит данные по просмотрам товаров на сайте. Есть проблема – просмотры одного customer_id не разбиты на сессии (появления на сайте). Мы хотим разместить сессии так, чтобы сессией считались все смежные просмотры, между которыми не более 3 минут.
Написать методом который создаст в Pandas DataFrame столбец session_id и проставит в нем уникальный int id для каждой сессии.
У каждого пользователя может быть по несколько сессий. Исходный DataFrame может быть большим – до 100 млн строк.



**Задание №2.**

В SQL базе данных есть продукты и категории. Одному продукту может соответствовать много категорий, в одной категории может быть много продуктов.
Напишите HTTP API через которое можно получить:
список всех продуктов с их категориями,
список категорий с продуктами,
список всех пар «Имя продукта – Имя категории».
Если у продукта нет категорий, то он все равно должен выводиться.
Если у категории нет продуктов, то она все равно должна выводиться.
Проект должен содержать docker-compose.yml файл, через который можно запустить сервис и проверить его работу.


**NOTE**:
For run use the next command in terminal and open http://localhost:8000/
```
~/mindbox> docker-compose up
```
It builds postgres with dummy data and django server with required by task lists from DB in web-browser:

![Screenshot from 2022-11-03 12-06-35](https://user-images.githubusercontent.com/63195531/199705954-76219910-e107-4397-8118-a9d85375965d.png)
