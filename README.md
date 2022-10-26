GET
/api/product/
HTTP 200 OK
С помощью этого метода мы получаем данные с таблицы 'Product' с полями: "id", "price_nds", "storage", "category", "name", "price", "description".
HTTP 404 Not Found
Вернется поле: "detail": "Страница не найдена."

POST
/api/product/
HTTP 201 Created
{
    "name": "asd123",
    "price": 1232,
    "description": "test",
    "storage": 1,
    "category": 1
}
HTTP 400 Bad Request
Если какие то поля заполнены с ошибками.

PATCH
/api/product/{id}/
HTTP 200 OK
{
    "name": "asd123",
    "price": 1232,
    "description": "test",
    "storage": 1,
    "category": 1
}
Если id указано неверно то выпадет такая ошибка:
HTTP 404 Not Found
{
    "detail": "Страница не найдена."
}

DELETE
/api/product/{id}/
HTTP Status 204 No Content
При неправильном запросе ответ будет:
HTTP 405 Method Not Allowed

GET
/api/category/
HTTP 200 OK
С помощью этого метода мы получаем данные с таблицу 'Category' с полем: "name".
HTTP 404 Not Found
Вернется поле: "detail": "Страница не найдена."

POST
/api/category/
HTTP 201 Created
{
    "name": "asd123",
}
HTTP 400 Bad Request
Если поле заполнено не верно.

PATCH
/api/category/{id}/
HTTP 200 OK
{
    "name": "asd123"
}
Если id указано неверно то выпадет такая ошибка:
HTTP 404 Not Found
{
    "detail": "Страница не найдена."
}

DELETE
/api/category/{id}/
HTTP Status 204 No Content
При неправильном запросе ответ будет:
HTTP 405 Method Not Allowed

GET
/api/storage/
HTTP 200 OK
С помощью этого метода мы получаем данные с таблицу 'Storage' с полем: "name".
HTTP 404 Not Found
Вернется поле: "detail": "Страница не найдена."

POST
/api/storage/
HTTP 201 Created
{
    "name": "asd123",
}
HTTP 400 Bad Request
Если поле заполнено не верно.

PATCH
/api/storage/{id}/
HTTP 200 OK
{
    "name": "asd123"
}
Если id указано неверно то выпадет такая ошибка:
HTTP 404 Not Found
{
    "detail": "Страница не найдена."
}

DELETE
/api/storage/{id}/
HTTP Status 204 No Content
При неправильном запросе ответ будет:
HTTP 405 Method Not Allowed

