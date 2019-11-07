# Backend de Discográfica

## Pasos para poder ejecutar el proyecto después de descargarlo
```
composer install
```

#### Crear archivo .env
Al ejecutar el siguiente comando se creará el archivo .env.example. Es necesario crear el archivo .env de forma manual en la raíz del proyecto y pegar todo el texto que se encuetra en el archivo .env.example, posteriormente cambiar el nombre de la base de datos en los parámetros del archivo.
```
copy NUL.env
```

#### Por último es necesario generar una clave única de nuestro proyecto. La generamos usando el siguente comando.
```
php artisan key:generate
```

## Pasos para crear las tablas de la base de datos

#### Antes de ejecutar el siguiente comando es necesario tener creada la base de datos (discografica)
```
php artisan migrate
```

## Notas adicionales

#### Crear proyecto de laravel
```
laravel new nombre_de_proyecto
```

#### Sección de ayuda para la creación de modelos
```
php artisan make:model --help
```

#### Crear un Modelo, Controlador, migración y factory
```
php artisan make:model Product --all
```

#### Listar las rutas
```
php artisan route:list
```

#### Sección de ayuda para la creación de controladores
```
php artisan make:controller --help
```

#### Crear controladores para modelos ya existentes. Por ejemplo. User
```
php artisan make:controller UserController -m User
```
  
#### Borrar toda la estructura de la base de datos y volverla a crear desde cero
```
php artisan migrate:fresh
```
  
#### Ubicación de archivos principales
* Controlador: app/Http/Controllers
* Modelo: app/
* Migración: database/migrations
* Factory: database/factories
* Rutas para api: routes/api.php