# SQL — Шпаргалка QA

## Основные команды

### SELECT — получить данные
SELECT * FROM users;

### WHERE — фильтрация
SELECT * FROM users
WHERE city = 'Москва';

### ORDER BY — сортировка
SELECT * FROM users
ORDER BY name ASC;

### LIMIT — ограничение количества
SELECT * FROM users
LIMIT 10;

### JOIN — объединение таблиц
SELECT orders.id, users.name
FROM orders
JOIN users ON orders.user_id = users.id;

### GROUP BY — группировка
SELECT city, COUNT(*)
FROM users
GROUP BY city;

---

## Быстрые правила

- Строки в одинарных кавычках: 'Москва'
- ASC — по возрастанию (А→Я)
- DESC — по убыванию (Я→А)
- * — все столбцы
