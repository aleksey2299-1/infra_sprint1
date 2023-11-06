## Проект Kittygram

Посмотреть на котиков и/или похвастаться своим(своими).

Чтобы похвастаться необходимо зарегистрироваться


### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:
````
got clone git@github.com:aleksey2299-1/infra_sprint1.git

cd infra_sprint1
````
Cоздать и активировать виртуальное окружение:
````
python3 -m venv venv

source venv/bin/activate

python3 -m pip install --upgrade pip
````
Установить зависимости из файла requirements.txt:
````
pip install -r requirements.txt
````
Выполнить миграции:
````
python3 backend/manage.py migrate
````
Запустить проект:
````
python3 backend/manage.py runserver
````
Backend доступен по адресу localhost:8000/

Установить пакетный менеджер npm:
````
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - &&\
sudo apt install -y nodejs
````
Установить зависимости для frontend'а:
````
cd frontend
npm i
````
Запустить frontend:
````
npm run start
````
Frontend доступен по адресу localhost:3000/

### Как начать?

Запустить вместе backend и frontend.

Перейте по адресу localhost:3000/

### Доступ по Api

__Чтобы увидеть информацию нужно зарегистрироваться:__

в теле запроса передать username и password:
````
localhost:8000/api/users/
````
получить token:
````
localhost:8000/api/token/login/
````


Посмотреть всеx котиков:
````
localhost:8000/api/cats/
````

Посмотреть конкретного котика:
````
localhost:8000/api/cats/<номер_котика>/
````

Посмотреть все достижения:
````
localhost:8000/api/achievements/
````

Посмотреть конкретное достижение:
````
localhost:8000/api/achievements/<номер_достижения>/
````
