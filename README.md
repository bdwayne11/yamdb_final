![workflow](https://github.com/bdwayne11/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg?branch=master&event=push)


***Как запустить проект:***
Клонировать репозиторий и перейти в него в командной строке:


git@github.com:bdwayne11/infra_sp2.git
cd infra


Cоздать и активировать виртуальное окружение:
```
git@github.com:bdwayne11/infra_sp2.git
cd infra
```

***Создать докер контейнеры:***

```
docker-compose up -d --build
```

***Развернуть докер контейнер***

```
docker-compose up
```

***Собрать статику и выполнить миграции:***

```
docker-compose exec web python manage.py migrate
docker-compose exec web python manage.py createsuperuser
docker-compose exec web python manage.py collectstatic --no-input
```

***Пример использования апи:***

```
GET-запрос на /api/v1/titles/ (получить все произведения)
```

```
POST-запрос на /api/v1/titles/ (добавление произведений, только для админа)
```

***Автор проекта Владислав Бойко***

