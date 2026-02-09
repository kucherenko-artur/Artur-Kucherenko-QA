HTTP 302 Redirect + Automatic Follow

Goal: Understand the difference between what we see in the console (final status) and what appears in the Network tab (redirect chain).

Request

Endpoint: https://httpbin.org/status/302 (redirects to /redirect/1)

Tool: Chrome DevTools → Console / Network

Method: See screenshots (Console/Network)

Expected Result

The Network tab should show a 302 status with a Location header, while the final request after the automatic follow may end with 200.

Actual Result

The console shows Status: 200 (final status after the follow), while in the Network tab you can see 302 Found and Location: /redirect/1.

Evidence

Screenshots are located in the evidence/ folder.

Notes

This is a training case for a QA portfolio (API/DevTools).

In a real project, this section would also include: reproduction steps, environment (OS/Browser), priority/severity, etc.
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
