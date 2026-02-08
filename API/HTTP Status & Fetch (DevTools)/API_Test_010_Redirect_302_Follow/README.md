# HTTP 302 Redirect + автоматический follow

**Цель:** Понять разницу между тем, что видим в console (итоговый status) и тем, что видно в Network (цепочка редиректов).

## Запрос
- **Endpoint:** `https://httpbin.org/status/302  (redirects to /redirect/1)`
- **Инструмент:** Chrome DevTools → Console / Network
- **Метод:** см. скриншоты (Console/Network)

## Ожидалось
В Network должен быть 302 с Location, а итоговый запрос после follow может закончиться 200.

## Фактически
В console выведен Status: 200 (итог после follow), в Network видно 302 Found и Location: /redirect/1.

## Доказательства
Скриншоты в папке `evidence/`.

## Заметки
- Это учебный кейс для портфолио QA (API/DevTools).
- В реальном проекте сюда бы добавили: шаги воспроизведения, окружение (OS/Browser), приоритет/севериити, и т.п.
