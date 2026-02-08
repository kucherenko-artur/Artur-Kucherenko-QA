# POST JSON request (fetch) -> 200 OK

**Цель:** Сделать POST с JSON body через fetch, проверить headers/payload в Network и что сервер эхо-возвращает данные.

## Запрос
- **Endpoint:** `https://httpbin.org/post`
- **Инструмент:** Chrome DevTools → Console / Network
- **Метод:** см. скриншоты (Console/Network)

## Ожидалось
Status = 200; Request Payload содержит отправленный JSON; Response (httpbin) включает отправленные поля.

## Фактически
Status Code: 200 OK; Request Payload показывает user/role/message.

## Доказательства
Скриншоты в папке `evidence/`.

## Заметки
- Это учебный кейс для портфолио QA (API/DevTools).
- В реальном проекте сюда бы добавили: шаги воспроизведения, окружение (OS/Browser), приоритет/севериити, и т.п.
