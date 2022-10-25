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

