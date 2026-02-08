# HTTP 500 Internal Server Error

**Цель:** Проверить, как Fetch отображает 5xx и что статус доступен через r.status.

## Запрос
- **Endpoint:** `https://httpbin.org/status/500`
- **Инструмент:** Chrome DevTools → Console / Network
- **Метод:** см. скриншоты (Console/Network)

## Ожидалось
Status = 500, в консоли может появиться сообщение об ошибке запроса, но r.status читается.

## Фактически
В консоли: GET ... 500 (Internal Server Error) и Status: 500.

## Доказательства
Скриншоты в папке `evidence/`.

## Заметки
- Это учебный кейс для портфолио QA (API/DevTools).
- В реальном проекте сюда бы добавили: шаги воспроизведения, окружение (OS/Browser), приоритет/севериити, и т.п.
