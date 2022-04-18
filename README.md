# api_yamdb 

api_yamdb предоставляет API для достпупа к базе данных произведений искусства и отзывов к ним и позволяет:
* просматривать категории и жанры произведений искусства
* просматривать и создавать отзывы к произведениям 
* оставлять комментарии к отзывам
* пользователи с правами администратора может создавать и обновлять категории и жанры


### Использованные технологии:
 Python 3.7, Django 2.2.16, DRF 3.12.4, Simple JWT, Pytest

### Установка:  

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/vitalyuvv/api_yamdb.git
```

```
cd api_yamdb
```

Cоздать и активировать виртуальное окружение:

```
python -m venv env
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate
```

Запустить проект:

```
python manage.py runserver
```
## Пример работы с API проекта Yamdb (v1)

#### Получение списка отзывов:
```
GET-запрос http://127.0.0.1:8000/api/v1/titles/{title_id}/reviews/
```
#### Создание нового отзыва
```
POST-запрос http://127.0.0.1:8000/api/v1/titles/{title_id}/reviews/
```
#### Обновление своего отзыва по id
```
PATCH-запрос: http://127.0.0.1:8000/api/v1/titles/{title_id}/reviews/{review_id}/
```



### Документация:
Доступна после запуска проекта [здесь](https://127.0.0.1:8000/redoc/)


### Авторы проекта:
  Виталий Усенко: https://github.com/vitalyuvv

  Юрий Ребрик: https://github.com/gkirber

  Александр Плисков: https://github.com/Glaser1



Проект распространяется под лицензией BSD
