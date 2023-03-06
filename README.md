# aula

### comandos para limpeza de cache, config e view
```
php artisan config:clear
php artisan cache:clear
php artisan view:clear
```

### Instala dependências
```
composer install
```

### Faz uma cópia do arquivo de exmplo e cria o .ENV
```
copy .env.example .env
```

### Gerar a app_key no arquivo .env
```
php artisan key:generate
```

### Criação de um link simbólico com o storage
```
php artisan storage:link
```


### Model
```
php artisan make:model NomeDoModel
```

#### Cria controller com resource (CRUD)
```
php artisan make:controller AlgumaController --resource
```

#### Cria Migration
```
php artisan make:migration create_produtos_table
```

#### Roda a migrate
```
php artisan migrate
```

#### Cria seed 
```
php artisan make:seeder ProdutoSeeder
```

#### Roda o seed
```
php artisan db:seed
```

### Roda a migrate e seed
```
php artisan migrate:refresh --seed
```








# utilidades

## Text2bin - Conversor de Texto para Binário
https://github.com/andreneves/utilidades/tree/main/Text2bin



ROUTES

// ------------------------------ PRODUTO -----------------------------
```
//listar todos os produtos
Route::get('/produto', [ProdutoController::class, 'index'])->name('produto.index');

Route::get('/produto/{id}', [ProdutoController::class, 'show'])->name('produto.show');

// create
Route::get('/produto/create', [ProdutoController::class, 'create'])->name('produto.create');
// store
Route::post('/produto/create', [ProdutoController::class, 'store'])->name('produto.store');

//edit
Route::get('/produto/{id}/edit', [ProdutoController::class, 'edit'])->name('produto.edit');
// update
Route::put('/produto/{id}', [ProdutoController::class, 'update'])->name('produto.update');

// delete
Route::delete('/produto/{id}', [ProdutoController::class, 'destroy'])->name('produto.delete');

// ------------------------------ PRODUTO -----------------------------
```