# Comparison of mobile operators tariffs 

The program accepts the filter values selected by the user and
offers a list of rates with a small spread of values to increase 
options. 
Each line with the proposed tariff shows additional options (if any) and a link to the page of the operator.

## Technology stack in use

* Python
* Flask
* SQLAlchemy
* база данных SQLite.

## Installation

Download the project from github:

```
git clone https://github.com/theoneman44/operator_comparing
```

Create the virtual environment you need for your system and install the dependencies:

```
pip install -r requirments.txt
```

Create a config.py file and set the base variables in it:

```
basedir = os.path.abspath(os.path.dirname(__file__))
SQLALCHEMY_DATABASE_URI = 'sqlite:///' + os.path.join(basedir, '..', 'tarifs.db')
SQLALCHEMY_TRACK_MODIFICATIONS = False
UPLOAD_FOLDER = './images'
SECRET_KEY = "Ваш ключ"
```

## Run the program

To run the program, run the `run` command from the directory where the downloaded program is located.

### P.S.
For the correct work of the program the database file `tarifs.db` filled according to the parameters of the models is required. 
At the moment the automatic filling of the database is in development.

# Сравнение тарифов мобильных операторов

Программа принимает значения фильтра выбранные пользователем и
предлагает список тарифов с небольшим разбросом значений для увеличения 
вариантов. 
В каждой строке с предлагаемым тарифом показаны дополнительные опции(при наличии) и ссылка на страницу оператора.

## Используемый стек технологий

* Python
* Flask
* SQLAlchemy
* база данных SQLite.

## Установка

Скачайте проект с github:

```
git clone https://github.com/theoneman44/operator_comparing
```
Создайте виртуальное окружение, необходимое для Вашей системы, и установите зависимости:

```
pip install -r requirments.txt
```

Создайте файл config.py и задайте в нем базовые переменные:

```
basedir = os.path.abspath(os.path.dirname(__file__))
SQLALCHEMY_DATABASE_URI = 'sqlite:///' + os.path.join(basedir, '..', 'tarifs.db')
SQLALCHEMY_TRACK_MODIFICATIONS = False
UPLOAD_FOLDER = './images'
SECRET_KEY = "Ваш ключ"
```

## Запуск программы

Для запуска программы выполните команду `run` из дирректории в которой находится скачанная программа.

### P.S.
Для корректной работы программы понадобится файл базы данных `tarifs.db` заполненный в соответствии с параметрами моделей. 
На данный момент автоматическое наполнение базы данных в разработке.
