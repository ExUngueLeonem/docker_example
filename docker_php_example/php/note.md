# Заметки по проекту 
## стягивание образа
docker build ./php
docker build -t my-php-app ./php

## запускаем контейнер
docker run -p 8001:80 -d my-php-app
-p 8001:80 -- host_port:container_port
-d -- запуск "фоном" в терминале см. Detached https://docs.docker.com/engine/reference/run/#detached--d
my-php-app - название имейджа (образа (изображения))

## опционально:
### Позволяет посмотреть, какие есть Images
docker images
### Выводит в терминал информацию по образам и контейнерам и прочее
docker info

## туториал 
https://www.youtube.com/watch?v=xuO8zv62HXM&list=PL0lO_mIqDDFX1c0JHogP5YuZdOVawoepS&index=5