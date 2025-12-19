# Простой HTTP-сервер с Nginx прокси

## Архитектура
- `backend`: Python HTTP-сервер на порту 8080 (доступен только внутри сети Docker).
- `nginx`: Обратный прокси на порту 80, перенаправляющий запросы на backend.

## Запуск
1. Клонировать репозиторий: `git clone https://github.com/timofeev174-hash/test`
2. Перейти в папку: `cd test`
3. Запустить: `docker compose up -d`

## Проверка
Выполните: `curl http://localhost`
Ожидаемый ответ: `Hello from Effective Mobile!`
