# Receipe_app_backend
Receipe app

docker-compose run --rm app sh -c "python manage.py collectstatic"
docker compose run --rm app sh -c "flake8"
docker compose run --rm app sh -c "python manage.py test"

docker compose run --rm app sh -c "django-admin startproject app ."

docker compose run --rm app sh -c "python manage.py startapp core"

add the template app to our project

docker compose run --rm app sh -c "python manage.py wait_for_db && flake8"

docker compose run --rm app sh -c "python manage.py makemigrations
docker compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"

69. Auth