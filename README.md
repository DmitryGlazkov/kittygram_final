![.github/workflows/main.yml](https://github.com/DmitryGlazkov/kittygram_final/actions/workflows/main.yml/badge.svg)

# Kittygram


## Описание проекта:
Социальная сеть для обмена фотографиями домашних питомцев. Позволят размещать фотографии своих питомцев, с указанием клички, года рождения, окраса и достижений, а также просматривать фотографии питомцев, добавленных другими пользователями. Доступна регистрация аккаунта, редактирование и удаление ранее внесённых данных, размещённых на сервисе питомцев.

## Использованные технологии:
 - Python
 - Django
 - Django REST framework
 - Nginx
 - Gunicorn
 - Docker
 - PostgreSQL
 - React
 - Certbot

## Как развернуть проект:

##### 1. Клонируйте репозиторий:
```
git clone git@github.com:DmitryGlazkov/kittygram_final.git
```

##### 2. Создайте и активируйте виртуальное окружение:
На Linux:
```
python3 -m venv env
source env/bin/activate
```

На Windows:
```
python -m venv venv
source venv/Scripts/activate
```

##### 3. В корневой директории создайте файл .env, внесите следующие данные:
```
POSTGRES_USER=kittygram_user
POSTGRES_PASSWORD=kittygram_password
POSTGRES_DB=kittygram
DB_HOST=db
DB_PORT=5432
SECRET_KEY=<your secret key>
DEBUG=True
```

##### 4. Установите зависимости:
```
cd backend
pip install -r requirements.txt
```

##### 5. Выполните миграции:
```
python manage.py migrate
```

##### 6. При необходимости создайте суперпользователя:
```
python manage.py createsuperuser
```

##### 7. Запустите локальный сервер:
```
python manage.py runserver
```


## Автор

[Дмитрий Глазков](https://github.com/DmitryGlazkov)
