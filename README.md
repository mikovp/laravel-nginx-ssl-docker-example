# Laravel 8/Php 7.4/MariaDB/Nginx ssl/Certbot/Docker-compose

## Production
```bash
#Copy .env
cp .env.example .env

#Start Docker 
docker-compose up -d

#Enter in container
docker-compose exec app bash

#Clear cache
php artisan optimize

#Generate app key
php artisan key:generate

#Install Node dependencies
npm install && npm run prod

#Nginx ssl for https Manual from https://www.github.com/staticfloat/docker-nginx-certbot
```
