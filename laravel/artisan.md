Artisan

https://laravel.com/docs/9.x/artisan


-- Comandos úteis

-- comandos para limpeza de cache e otimizacao
php artisan config:clear
php artisan config:cache
php artisan cache:clear
php artisan optimize

-- limpando as views do sistema
php artisan view:clear

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
Mostra o status de cada migration.
php artisan migrate:status

-- ROUTES
Podemos listar todas as rotas utilizando:
php artisan route:list

-- MAKE
cria uma nova classe controller;
php artisan make:controller NomeController
cria uma nova classe model
php artisan make:model Nome
cria um novo arquivo de migração;
php artisan make:migration
Cria um aquivo de migration chamado add_votes_to_users_table para a alteração de uma tabela chamada users.
php artisan make:migration add_votes_to_users_table --table=users

Cria uma nova classe chamada CheckAge.
php artisan make:middleware CheckAge

Cria um aquivo de migration chamado create_users_table para a criação de uma tabela chamada users
php artisan make:migration create_users_table --create=users

Cria uma estrutura básica de login e registro de usuário com views e routes.
php artisan make:auth

Cria uma nova seeder chamada UsersTableSeeder.
php artisan make:seeder UsersTableSeeder

Cria uma nova classe de teste chamada UserTest.
php artisan make:test UserTest

Cria uma nova form request class chamada StoreBlogPost.
php artisan make:request StoreBlogPost

-- route:
O route possibilita a criação de rotas, tornando a aplicação mais segura.Alguns exemplos:
php artisan route:cache : cria um arquivo de rota cache de registro rápido;
php artisan route:clear : remove o arquivo de rota do cache;
php artisan route:list : apresenta todas as rotas registradas na aplicação;

-- abre o servidor
php artisan serve


Cria uma migration para gerar uma tabela de cache.
php artisan cache:table

Popula com dados as tabelas do framework de acordo os arquivos de seeds.
php artisan db:seed

Remove os arquivos compilados
php artisan clear-compiled

Este comando é usado para criar uma nova classe de política.
php artisan make: policy Policy_Name

Este comando é usado para criar uma nova classe de email.
php artisan make: mail EMail_Class_Name
