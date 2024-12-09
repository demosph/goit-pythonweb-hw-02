# ДЗ Тема: Основи технології Docker

Створіть віртуальне оточення то встановіть необхідні бібліотеки

```bash
pip install -r requirements.txt
```

Запуск:

```bash
python main.py
```

Запуск середовища Docker

```
docker-compose up
```

Приклад виконання:
```
postgres  | 2024-12-09 13:09:16.198 UTC [1] LOG:  database system is ready to accept connections
app-1     | INFO:     Started server process [8]
app-1     | INFO:     Waiting for application startup.
app-1     | INFO:     Application startup complete.
app-1     | INFO:     172.18.0.1:47846 - "GET / HTTP/1.1" 200 OK
app-1     | INFO:     172.18.0.1:47846 - "GET /style.css HTTP/1.1" 200 OK
app-1     | INFO:     172.18.0.1:47844 - "GET /main.js HTTP/1.1" 200 OK
app-1     | INFO:     172.18.0.1:47844 - "GET /favicon.ico HTTP/1.1" 404 Not Found
app-1     | 2024-12-09 13:09:46,542 INFO sqlalchemy.engine.Engine select pg_catalog.version()
app-1     | 2024-12-09 13:09:46,542 INFO sqlalchemy.engine.Engine [raw sql] {}
app-1     | 2024-12-09 13:09:46,544 INFO sqlalchemy.engine.Engine select current_schema()
app-1     | 2024-12-09 13:09:46,544 INFO sqlalchemy.engine.Engine [raw sql] {}
app-1     | 2024-12-09 13:09:46,546 INFO sqlalchemy.engine.Engine show standard_conforming_strings
app-1     | 2024-12-09 13:09:46,546 INFO sqlalchemy.engine.Engine [raw sql] {}
app-1     | 2024-12-09 13:09:46,547 INFO sqlalchemy.engine.Engine BEGIN (implicit)
app-1     | 2024-12-09 13:09:46,548 INFO sqlalchemy.engine.Engine SELECT 1
app-1     | 2024-12-09 13:09:46,549 INFO sqlalchemy.engine.Engine [generated in 0.00039s] {}
app-1     | 2024-12-09 13:09:46,551 INFO sqlalchemy.engine.Engine ROLLBACK
app-1     | INFO:     172.18.0.1:47844 - "GET /healthchecker HTTP/1.1" 200 OK
app-1     | 2024-12-09 13:10:03,040 INFO sqlalchemy.engine.Engine BEGIN (implicit)
app-1     | 2024-12-09 13:10:03,041 INFO sqlalchemy.engine.Engine SELECT 1
app-1     | 2024-12-09 13:10:03,041 INFO sqlalchemy.engine.Engine [cached since 16.49s ago] {}
app-1     | 2024-12-09 13:10:03,042 INFO sqlalchemy.engine.Engine ROLLBACK
app-1     | INFO:     172.18.0.1:34934 - "GET /healthchecker HTTP/1.1" 200 OK
app-1     | INFO:     172.18.0.1:34934 - "GET / HTTP/1.1" 200 OK
app-1     | 2024-12-09 13:10:06,700 INFO sqlalchemy.engine.Engine BEGIN (implicit)
app-1     | 2024-12-09 13:10:06,700 INFO sqlalchemy.engine.Engine SELECT 1
app-1     | 2024-12-09 13:10:06,701 INFO sqlalchemy.engine.Engine [cached since 20.15s ago] {}
app-1     | 2024-12-09 13:10:06,702 INFO sqlalchemy.engine.Engine ROLLBACK
app-1     | INFO:     172.18.0.1:34934 - "GET /healthchecker HTTP/1.1" 200 OK
```