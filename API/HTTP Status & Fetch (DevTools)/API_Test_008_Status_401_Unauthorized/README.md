# HTTP 401 Unauthorized (Basic Auth prompt)

**Цель:** Понять поведение браузера/Fetch при запросе к эндпоинту, который требует Basic Auth.

## Запрос
- **Endpoint:** `https://httpbin.org/basic-auth/user/passwd`
- **Инструмент:** Chrome DevTools → Console / Network
- **Метод:** см. скриншоты (Console/Network)

## Ожидалось
Сервер должен вернуть 401 Unauthorized (или 200 при корректных кредах). Браузер может показать Basic Auth prompt.

## Фактически
Получен 401 Unauthorized, браузер показал окно ввода логина/пароля.

## Доказательства
Скриншоты в папке `evidence/`.

## Заметки
- Это учебный кейс для портфолио QA (API/DevTools).
- В реальном проекте сюда бы добавили: шаги воспроизведения, окружение (OS/Browser), приоритет/севериити, и т.п.
