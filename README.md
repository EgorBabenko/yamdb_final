# Проект API YAMDB
## Общее описание
Учебный проект api сервиса для публикации отзывов о произведениях разных жанров
## Технологии:
- Python 3.7
- Django Rest Framework
- Postgres
- Docker
### Документация доступна по эндпойнту redoc/

## Локальный старт
После клонирования репозитория выполните следующие действия:
- Создать файл .env в директории /infra/ со следующим содержимым:

DB_ENGINE=django.db.backends.postgresql

DB_NAME= # название БД\ POSTGRES_USER= # ваше имя пользователя

POSTGRES_PASSWORD= # пароль для доступа к БД

DB_HOST=db

DB_PORT=5432\

- Из папки infra/ выполнить команду $ docker-compose up -d --build
- $ docker-compose exec web python manage.py migrate
- docker-compose exec web python manage.py collectstatic --no-input
- $ docker-compose exec web python manage.py createsuperuser (создание суперюзера)

## Об авторе
Автор - Бабенко Егор, студент 31 когорты курса "Python разработчик" Яндекс-Практикума.
Соискатель на вакансии Junior Python Developer

##  MIT License
 Copyright (c) 1998, 1999, 2000 Thai Open Source Software Center Ltd
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
 the following conditions:
 
 The above copyright notice and this permission notice shall be included
 in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.