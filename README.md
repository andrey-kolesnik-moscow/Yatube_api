Описание проекта

Проект создан как серверное приложение для публикации постов с расширенным функционалом. Это полноценное API, поддерживающее работу с любыми пользовательскими интерфейсами. Чтение публикаций и комментариев доступно для всех пользователей сети интернет сразу "из коробки". А после прохождения короткого процесса авторизации и получения токена для Вас открывается возможность стать непосредственным участником этого проекта. То есть Вы сможете публиковать посты, оставлять комментарии, вступать в группы и подписываться на других авторов.  

Адрес проекта на гитхаб:
https://github.com/andrey-kolesnik-moscow/api_final_yatube

Как запустить проект

Клонировать репозиторий и перейти в него в командной строке:
git clone git@github.com:andrey-kolesnik-moscow/api_final_yatube.git
cd api_final_yatube

Cоздать и активировать виртуальное окружение:
python -m venv env
source env/bin/activate

Установить зависимости из файла requirements.txt:
python -m pip install --upgrade pip
pip install -r requirements.txt

Выполнить миграции:
python manage.py migrate

Запустить проект:
python manage.py runserver

Примеры запросов доступны сразу после запуска сервера по адресу:
http://<server_ip:port>/redoc/