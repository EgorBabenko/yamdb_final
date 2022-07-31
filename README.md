# Yamdb - REST API  сервис для отзывов о произведениях разныж жанров

![Build Status](https://github.com/EgorBabenko/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

### Проект доступен по адресам:
- http://51.250.111.195/redoc - документация API
- http://51.250.111.195/admin - админка

## Локальный старт:
1. Клонируйте репозиторий на локальный компьютер
```
git clone <адрес репозитория>
```
2. Установите виртуальное окружение и зависимости
```
python -m venv venv
pip install -r requirements.txt 
```
3. Находясь в директории /api_yamdb выполните в терминале:
- Миграции БД:
```
python manage.py migrate
```
- Сбор статики:
```
python manage.py python manage.py collectstatic --no-input
```
- Создание суперпользователя:
```
python manage.py python manage.py createsuperuser
```

##Технологии проекта
 - Python 3.7
 - Django Rest Framework
 - Docker
 - Реализовано CI/CD (Docker Compose, GitHub Actions)

##Об авторе:
Автор - Бабенко Егор, студент 31 когорты курса "Python разработчик" Яндекс-Практикума. Соискатель на вакансии Junior Python Developer


##MIT LIcense
Copyright (c) 1998, 1999, 2000 Thai Open Source Software Center Ltd

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.