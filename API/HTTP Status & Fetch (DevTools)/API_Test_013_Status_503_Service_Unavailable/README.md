# HTTP 503 Service Unavailable

**Цель:** Отработать 503 и посмотреть заголовки/тип ответа в Network.

## Запрос
- **Endpoint:** `https://httpbin.org/status/503`
- **Инструмент:** Chrome DevTools → Console / Network
- **Метод:** см. скриншоты (Console/Network)

## Ожидалось
Status = 503; в Network можно увидеть заголовки ответа (Content-Type и т.д.).

## Фактически
В Network отображается 503 Service Unavailable; headers видны.

## Доказательства
Скриншоты в папке `evidence/`.

## Заметки
- Это учебный кейс для портфолио QA (API/DevTools).
- В реальном проекте сюда бы добавили: шаги воспроизведения, окружение (OS/Browser), приоритет/севериити, и т.п.
