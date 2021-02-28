Сборка для поднятия локального сервера разработки

* PHP: php:7.3-fpm-stretch
* NGINX: nginx:alpine
* БД: postgres:11


NGINX настроен так, чтобы каждую папку в apps считать поддоменом *.dev.localhost

Доступные команды:
* make up - "включить" все контейнеры
* make down - "выключить" все контейнеры
* make restart - "перезагрузка" контейнеров
* domains.sh - вывод всех локальных сайтов в виде ссылок
* copy_arti.sh {PROJECT_DIR} - копирует обертку над artisan для laravel, чтобы artisan команды выполнять внутри контейнера