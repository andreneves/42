Artisan

https://laravel.com/docs/9.x/artisan


-- Comandos úteis

-- comandos para limpeza de cache e otimizacao
php artisan config:clear
php artisan config:cache
php artisan cache:clear
php artisan optimize


-- lista de comandos e versao
php artisan list

-- lista todas as ajudas para o Framework.
php artisan help

-- Abre o tinker
php artisan tinker


php artisan migrate

php artisan migrate:refresh --seed

-- Controller

php artisan make:controller NomeController
Controlador com resource (CRUD)
php artisan make:controller AlgumaController --resource

-- Model
php artisan make:model Alguma
Model com migrate
php artisan make:model Alguma --migration

-- Migrate
php artisan make:migration create_algumas_table
php artisan migrate
Já para ver o status, usamos:
php artisan migrate:status

-- ROUTES
Podemos listar todas as rotas utilizando:
php artisan route:list

-- MAKE
php artisan make:controller : cria uma nova classe controller;
php artisan make:model : cria uma nova classe model;
php artisan make:migration : cria um novo arquivo de migração;

-- route:
O route possibilita a criação de rotas, tornando a aplicação mais segura.Alguns exemplos:
php artisan route:cache : cria um arquivo de rota cache de registro rápido;
php artisan route:clear : remove o arquivo de rota do cache;
php artisan route:list : apresenta todas as rotas registradas na aplicação;

-- abre o servidor
php artisan serve
