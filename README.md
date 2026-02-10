[![Main Kittygram workflow](https://github.com/this-is-tania/kittygram_final/actions/workflows/main.yml/badge.svg)](https://github.com/this-is-tania/kittygram_final/actions/workflows/main.yml)

# Проект Kittygram

Kittygram — веб-приложение для публикации информации о котиках. Пользователи могут добавлять информацию о своих котиках, загружать фотографии, отмечать достижения котиков, а также просматривать записи, созданные другими пользователями.

## Технологии проекта

- Фронтенд: React
- Бэкенд: Django Rest Framework
- База данных: PostgreSQL
- Nginx
- Docker
- Gunicorn
- Github actions

# Запуск проекта

## Локальный запуск

1. Скопирайте проект с GitHub, настройте виртуальное окружение и установите зависимости
```commandline
git clone https://github.com/this-is-tania/kittygram_final.git
cd kittygram_final
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
2. Выполните миграции:

```commandline
python manage.py migrate

```

3. Запустите проект:

```commandline
python manage.py runserver
```
## Запуск в Docker

```commandline
docker-compose up --build
```
После запуска приложение будет доступно по адресу:

```commandline
http://localhost:9000
```

## Переменные окружения

Пример структуры файла .env

```commandline
POSTGRES_DB=kittygram
POSTGRES_USER=kittygram_user
POSTGRES_PASSWORD=kittygram_password
DB_NAME=kittygram
```