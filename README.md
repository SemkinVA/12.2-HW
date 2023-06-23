# 12.2-HW

### Домашнее задание к занятию 12.2 - "Работа с данными (DDL/DML)" - Семкин Вячеслав
***

### Задание 1
1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

1.2. Создайте учётную запись sys_temp. 

1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)

1.4. Дайте все права для пользователя sys_temp. 

1.5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

1.6. Переподключитесь к базе данных от имени sys_temp.

Для смены типа аутентификации с sha2 используйте запрос: 
```sql
ALTER USER 'sys_test'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
```
1.6. По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.

1.7. Восстановите дамп в базу данных.

1.8. При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)

*Результатом работы должны быть скриншоты обозначенных заданий, а также простыня со всеми запросами.*


**Ответ:**

1.1 Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

![1-1](https://github.com/SemkinVA/12.2-HW/blob/main/1-1.png)


1.2 Создайте учётную запись sys_temp. 

![1-2](https://github.com/SemkinVA/12.2-HW/blob/main/1-2.png)


1.3 Выполните запрос на получение списка пользователей в базе данных. (скриншот)

![1-3](https://github.com/SemkinVA/12.2-HW/blob/main/1-3.png)


1.4 Дайте все права для пользователя sys_temp.

![1-4](https://github.com/SemkinVA/12.2-HW/blob/main/1-4.png)


1.5 Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

![1-5](https://github.com/SemkinVA/12.2-HW/blob/main/1-5.png)


1.6 Переподключитесь к базе данных от имени sys_temp.

![1-6](https://github.com/SemkinVA/12.2-HW/blob/main/1-6.png)


1.7 Восстановите дамп в базу данных.

![1-7](https://github.com/SemkinVA/12.2-HW/blob/main/1-7.png)


1.8 При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)

![1-8-1](https://github.com/SemkinVA/12.2-HW/blob/main/1-8-1.png)

![1-8-2](https://github.com/SemkinVA/12.2-HW/blob/main/1-8-2.png)


***

### Задание 2
Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца: в первом должны быть названия таблиц восстановленной базы, во втором названия первичных ключей этих таблиц. Пример: (скриншот/текст)
```
Название таблицы | Название первичного ключа
customer         | customer_id
```

**Ответ:**

|Название таблицы | Название первичного ключа|Количество первичных ключей|
|---|---|---|
|paymant|	paymant_id|	1|
|rental|	rental_id|	1|
|costorer|	costorer_id|	1|
|inventory|	inventory_id|	1|
|store|	store_id|	1|
|staff|	staff_id|	1|
|address|	address_id|1|	
|city|	city_id|	1|
|country|	country_id|1|	
|film|	film_id|	1|
|language|	language_id|	1|
|film_actor|	film_id	и actor_id| 2|
|actor|	actor_id|	1|
|film_category|	film_id	и category_id| 2|
|category|	category_id|	1|
|film_text|	film_text_id|	1|
|sales_by_film_category|		|	0|
|sales_by_store	|	|	0|
|acrot_info	|	|0|
|folm_list	|		|0|
|nicer_but_slower_folm_list		|	|0|
|stuff_lost		|	|0|
|costomer_list|	|	0|	



