# PHP API для MySQL

Эти файлы нужно загрузить на ваш хостинг в отдельную папку (например, `/api/`).

## Установка

1. Загрузите все PHP файлы на хостинг
2. Отредактируйте `config.php`:
   - `DB_HOST` - хост базы данных (обычно `localhost`)
   - `DB_NAME` - имя базы данных
   - `DB_USER` - логин MySQL
   - `DB_PASS` - пароль MySQL
   - `ADMIN_USER` - логин для админки
   - `ADMIN_PASS` - пароль для админки

3. Откройте в браузере: `https://yoursite.com/api/install.php`
   - Это создаст все необходимые таблицы

4. В приложении перейдите на `/admin/login` и введите:
   - URL вашего API (например, `https://yoursite.com/api`)
   - Логин и пароль из config.php

## Файлы API

- `config.php` - конфигурация БД и авторизации
- `install.php` - создание таблиц
- `auth.php` - авторизация
- `companies.php` - CRUD для компаний
- `events.php` - CRUD для событий
- `founders.php` - CRUD для основателей

## Безопасность

⚠️ **Важно:**
- Измените логин и пароль в config.php
- Ограничьте доступ к install.php после установки
- Используйте HTTPS
