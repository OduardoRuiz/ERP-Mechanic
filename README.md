# ERP para Oficina Mecânica

## Stack
- Laravel 12
- Vue.js 3
- MySQL 8
- Docker

## Desenvolvimento

1. Clone o repositório
2. Execute: `docker-compose up -d --build`
3. Configure o .env: `cp src/.env.example src/.env`
4. Gere a chave: `docker exec -it erp_app php artisan key:generate`
5. Execute migrações: `docker exec -it erp_app php artisan migrate`
6. Acesse: http://localhost:8082

## Comandos úteis
- `docker-compose exec app composer install` - Instalar dependências PHP
- `docker-compose exec app npm install` - Instalar dependências Node
- `docker-compose exec app php artisan make:model Product -mcr` - Criar model
