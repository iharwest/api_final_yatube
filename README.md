# api_final
api_final_yatube - REST API для проекта социальной сети Yatube.

### Системные требования
- Python 3.7+
- Works on Linux, Windows, macOS

### Технологии
Python 3.7
Django 2.2.19

### Запуск проекта:
Клонировать репозиторий и скопировать проект на рабочую машину через команду в терминале
GitBash или через Терминал bash в Visual Studio Code
```
git clone git@github.com:iharwest/api_final_yatube.git
```
Перейти в директорию, в которую сохранили клонированный проект 
```
cd api_final_yatube
```
Cоздать и активировать виртуальное окружение:
```
python -m venv venv
```
В Windows:
```
source venv/Scripts/activate
```
В macOS или Linux:
```
source venv/bin/activate
```
Установить зависимости из файла requirements.txt:
```
python -m pip install --upgrade pip
pip install -r requirements.txt
```
Выполнить миграции:
```
python manage.py migrate
```
Перейти в директорию с файлом manage.py и из нее запустить проект:
```
python manage.py runserver
```
Документация к проекту
----------
Документация для API после установки доступна по адресу ```/redoc/```.

Примеры запросов к API:
```
api/v1/posts/:(GET, POST) - получение списка всех публикаций или создание новой.

api/v1/posts/{post_id}/:(GET, PUT, PATCH, DELETE) - получение, редактирование, редактирование или удаление выбранной публикации по id.

api/v1/groups/:(GET) - получение списка всех групп.

api/v1/groups/{group_id}/:(GET) - получение информации о группе по id.

api/v1/posts/{post_id}/comments/:(GET, POST) - получение всех комментариев или их добавление к публикации.

api/v1/posts/{post_id}/comments/{comment_id}/:(GET, PUT, PATCH, DELETE) получение, редактирование или удаление комментария к публикации по id.

api/v1/jwt/create/:(POST) - передача логина и пароля, получение JWT-токена.

api/v1/jwt/refresh/:(POST) - обновление JWT-токена. 

api/v1/jwt/verify/:(POST) - проверка JWT-токена.
```