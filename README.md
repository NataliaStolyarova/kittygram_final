# Kittygram - социальная сеть с фотографиями котиков и их достижениями. Никаких собак!

## Используемые технологии:
- Python 3.9.13
- Django 3.2.3
- Django REST framework 3.12.4
- React
- JavaScript

## Как запустить проект Kittygram в режиме разработки:

* Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/NataliaStolyarova/kittygram_final.git
```

```
cd kittygram_final
```

* Запустить проект:

```
docker compose up
```

* Собрать и скопировать статику:

```
docker compose exec backend python manage.py collectstatic
```

```
docker compose exec backend cp -r /app/collected_static/. /static/static/
```

* Перейти по адресу http://127.0.0.1:9000/
