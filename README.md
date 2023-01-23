# API Yatube

# API социальной сети блогеров Yatube

REST API для проекта YaTube

У неаутентифицированных пользователей есть возможность получить посты пользователей соцсети, комментарии к постам, а также информацию о группах. Аутентифицированные пользователи могут добавлять посты и комментарии, подписываться на авторов. Также им доступно изменение и удаление своего контента.

Для аутентификации используются JWT-токены.

Технологии:
Python 3.7, Django 2.2, Django REST framework 3.12, библиотека Simple JWT - работа с JWT-токеном

# Как запустить проект
# Клонировать репозиторий и перейти в него в командной строке:

git clone https://github.com/sukhovarina/Yatube-API.git
cd yatube_api

# Cоздать и активировать виртуальное окружение:

python -m venv env
source venv/Scripts/activate

@ Установить зависимости из файла requirements.txt:

python -m pip install --upgrade pip
pip install -r requirements.txt

@ Выполнить миграции:

python manage.py migrate

# Запустить проект:

python manage.py runserver
