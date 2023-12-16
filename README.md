# Run Local
```sh
docker compose up -d
```
- access to http://localhost:58000

# Init

see: https://docs.docker.jp/compose/django.html

## Create Dockerfile for db
```sh
mkdir -p docker/postgres
touch docker/postgres/Dockerfile
```

## Create Dockerfile for app
```sh
mkdir -p docker/python
touch docker/python/Dockerfile
```

## Create docker-compose.yml
- db
- app

## Create Django Project
The app name is `sandbox`.

```sh
docker compose run app django-admin startproject sandbox .
```
