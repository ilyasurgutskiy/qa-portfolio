# BUG-003 — API пустой POST

**Title:** API принимает POST запрос с пустым телом и возвращает 201 вместо 400

## Steps to Reproduce
1. Открыть Postman Web
2. Создать POST запрос на https://jsonplaceholder.typicode.com/posts
3. В поле Body выбрать raw → JSON
4. Оставить тело пустым {}
5. Отправить запрос

## Expected Result
Сервер возвращает код 400 Bad Request

## Actual Result
Сервер возвращает код 201 и создаёт объект с id: 101

## Details
- **Severity:** Major
- **Priority:** High
- **Tool:** Postman Web
- **Browser:** Safari
- **Device:** iPad Pro M2
