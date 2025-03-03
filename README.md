# Домашнее задание к занятию «Работа с данными (DDL/DML)» - Макану Александр


### Задание 1

```sql
CREATE USER 'sys_temp'@'localhost' IDENTIFIED BY 'password';

SELECT user, host FROM mysql.user;

GRANT ALL PRIVILEGES ON *.* TO 'sys_temp'@'localhost' WITH GRANT OPTION;
FLUSH PRIVILEGES;

SHOW GRANTS FOR 'sys_temp'@'localhost';

SOURCE /home/osboxes/sakila-db/sakila-schema.sql;
SOURCE /home/osboxes/sakila-db/sakila-data.sql;

SHOW TABLES FROM sakila;

![screenshot1](img/task1-3.jpg)

![screenshot2](img/task1-5.jpg)

![screenshot3](img/task1-8.jpg)

### Задание 2

![screenshot4](img/task2.jpg)