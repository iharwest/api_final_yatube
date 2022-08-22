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