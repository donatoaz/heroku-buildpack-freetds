Heroku buildpack: FreeTDS
=======================

A Heroku Buildpack created to install [FreeTDS](http://www.freetds.org/) in your project. Allows for usage of [TinyTDS](https://github.com/rails-sqlserver/tiny_tds) on Heroku and was used succesfully to connect to a MS SQL Server 2005 database.

Este é um Buildpack criado para instalar o [FreeTDS](http://www.freetds.org/) em seu projeto. Permite o uso do [TinyTDS](https://github.com/rails-sqlserver/tiny_tds) no Heroku e foi usado com sucesso para conectar a um banco de dados MS SQL Server 2005.

Usage
-----

This buildpack was tested along with version v170 of heroku's standard ruby [buildpack](https://github.com/heroku/heroku-buildpack-ruby/releases/tag/v170). 

Add this repo *before* the ruby buildpack and you're good to go:

    $ heroku buildpacks:add --index 1 https://github.com/donatoaz/heroku-buildpack-freetds.git

To confirm, you can run

    $ heroku buildpacks
    
And see where it comes in your buildpack execution order

Uso
-----

Este buildpack foi testado contra a versão v170 do ruby buildpack padrão do heroku.

Adicione este repo *antes* do buildpack ruby e você está pronto para utilizar:

    $ heroku buildpacks:add --index 1 https://github.com/donatoaz/heroku-buildpack-freetds.git

Para confirmar, pode executar

    $ heroku buildpacks
    
E verificar a posição em que este buildpack será executado (deve ser antes do buildpack ruby)
