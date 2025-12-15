# HotelAPI

Данный API предназначен для управления данными 5* отеля

#Использованные технологии:
1. Django
2. Django REST Framework
3. drf-yasg
4. JWT (SimpleJWT)
5. SQLite

#Установка и запуск
1. Скачайте zip-файл и распакуйте в удобной для вас папке
2. Создайте виртуальную среду:</br>
   а)для Windows: python -m venv venv venv\Scripts\activate;</br>
   б)для Linux/Mac: python3 -m venv venv source venv/bin/activate</br>
3. Установите зависимости: pip install -r requirements.txt
4. Примените миграции: python manage.py migrate
5. Создайте суперпользователя: python manage.py createsuperuser
6. Запустите сервер: python manage.py runserver
7. Далее вам будет представлена страница с путями, чтобы начать работу с данными в Swagger, перейдите по пути: /swagger
8. Также не забудьте получить токен через путь /token отправив запрос: POST /api/token/ { "username": "admin", "password": "password" }
9. После для авторизации вставьте токен В Swagger: Bearer <access_token>
