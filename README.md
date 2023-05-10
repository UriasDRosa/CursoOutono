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

