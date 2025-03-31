# Веб-сервис для управления движением денежных средств (ДДС)

Этот проект представляет собой веб-приложение для управления движением денежных средств (ДДС), позволяющее пользователям создавать, редактировать, удалять и просматривать записи о транзакциях.

## Особенности

- Создание, редактирование и удаление записей о транзакциях.
- Просмотр списка всех транзакций с фильтрацией по дате, статусу, типу, категории и подкатегории.
- Управление справочниками: добавление, редактирование и удаление статусов, типов, категорий и подкатегорий.
- Логические зависимости между сущностями: подкатегории привязаны к категориям, категории привязаны к типам.

## Требования

- Python 3.x
- Django 3.x или выше
- SQLite (или другая реляционная база данных)

## Пометка

Проект находится в ветке master

## Установка

1. **Клонируйте репозиторий:**

   ```bash
   git clone https://github.com/z1eroRoma/Money_management.git
   cd money_management

## Создайте виртуальное окружение и активируйте его

python -m venv venv
source venv/bin/activate  # Для Windows: venv\Scripts\activate


## Установите зависимости

pip install -r requirements.txt


## Примите миграции базы данных

python manage.py makemigrations
python manage.py migrate


## Создайте суперпользователя для доступа к админке

python manage.py createsuperuser


## Запустите сервер

python manage.py runserver
