# HTTP 302 Redirect + Automatic Follow

## Purpose
Demonstrate how browsers automatically follow `302` redirects and why the final status shown in the **Console** may differ from the initial redirect response visible in **Network**.

## Request Details
- **Endpoint:** `https://httpbin.org/status/302` (redirects to `/redirect/1`)
- **Tool:** Chrome DevTools → Console / Network
- **Method:** See screenshots in the `evidence/` folder

## Expected Result
- The **first** request in the Network panel should return:
  - `302 Found`
  - A `Location` header (e.g., `/redirect/1`)
- After the automatic follow, the **final** request may return:
  - `200 OK`

This demonstrates how redirect chains work internally.

## Actual Result
- **Console:** Displays only the final status — `Status: 200`
- **Network:** Shows the redirect chain:
  - `302 Found`
  - `Location: /redirect/1`
  - Follow-up request ending with `200 OK`

## Evidence
Screenshots are located in the `evidence/` folder:
- Console output
- Network request list
- Redirect response headers

## Notes
- Training case for a QA portfolio (API/DevTools).
- In a real project, this would also include: reproduction steps, environment (OS/Browser), severity/priority, and additional logs (e.g., HAR).

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
