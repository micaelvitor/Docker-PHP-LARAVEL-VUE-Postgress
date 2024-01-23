# Laravel 8 & Vue 3 App com TypeScript

Ambiente de desenvolvimento Docker para Laravel 8.\* com:

- Nginx
- PostgreSQL
- PHP8.3
- Vue
- Node

## Instação

- Copie o arquivo `.env`: `cp .env.example .env`
- Configure as variaveis de ambiente no arquivo `.env`
- Rode o comando: `docker-compose up --build -d`
- Rode o container em modo bash: `docker exec -it Laravel_php /bin/sh`
- Dentro do container rode ss seguintes comandos:
- Dependencias do composer: `composer update && composer install`
- Gere a application key: `php artisan key:generate`
- Rode as migrations: `php artisan migrate`
- Rode os seeders: `php artisan db:seed`
- Instale as dependencias do javascript: `yarn`
- Compile os assets: `yarn dev` / `yarn watch`  
- De as permissões necessarias no storage do laravel: `chmod 777 -R ./storage`
- Agora você pode rodar o projeto no seu browswer na seguinte URL: `http://localhost:8000`

