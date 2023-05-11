# CursoOutono

Laravel, DBeaver, MySQL, Blade, Artisan, Composer.

# Requisitos

• Ter o XAMPP instalado.
Rodar o Apache e o MySQL.

## Criando o Projeto laravel com o composer

- (cmd) Na pasta qu se deseja criar o projeto.
composer create-project laravel/laravel "project.name".

composer require laravel/breeze.
php artisan breeze:install --dark

# Comandos

- Caminhar até o diretório do projeto pelo cmd.
php artisan serve - para iniciar o servidor do Laravel.

## Criando as migrations(tables do banco)

- Na pasta do Projeto.
php artisan make:migration "migration.name".

Após criar todas as migrations, no cmd, executar o comando: php artisan migrate.

php artisan make:controller "controller.name"

php artisan make:model "new.model.name" 

# Se for git clone

executar o composer install 

trocar o nome do arquivo .env.example para somente .env

gerar uma nova chave com o comando php artisan key:generate

rodar o npm install, npm run build e php artisan serve.

# Configurando as rotas/MVC

criar a rota para o arquivo, exemplo: Route::resource('/medico', 'App\Http\Controllers\MedicoController')->middleware(['auth', 'verified']);

criar o controller pelo cmd exemplo: php artisan make:controller MedicoController

importar o Model para o arquivo, exemplo: use App\Models\Medico;

criar uma function, como a index: 
`public function index(){
        $medicos = Medico::getAllMedicos();
        return view ('medicos.index', ['medicos' => $medicos]);
}`

Na pasta de layouts, criar uma pasta para a view "Medico" por exemplo, criar um arquivo "index.blade.php" dentro da pasta, criar o layout seguindo os padrões do laravel e do blade.
