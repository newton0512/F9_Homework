# F9_Homework

Напишите сервер на aiohttp, который:

1. Позволяет клиентам подключиться через веб-сокеты на сообщения (новости).
2. Может получать новые новости методом POST/news (предположим, что этот запрос нам отправляет другой сервис) и рассылать всем подключившимся клиентам.
3. Позволяет периодически проверять соединение между клиентом и сервером при помощи запросов, которые ничего не меняют.
4. Сделайте страницу, которая может отображать полученные от этого сервиса сообщения.


Подключение клиентов происходит по адресу http://localhost:8080.
Новости поступают в канал через post-запрос на адрес http://localhost:8080/news.
Для контроля соединения добавлен heartbeat на стороне сервера, на стороне клиента отправляется сообщение "ping", на которое ожидается ответ "pong".
