# laravel curso - migraciones

### migraciones

las migraciones son para indicar a través de Laravel la estructura de la base de datos

en Laravel no vamos tocar las consultas o sentencias a la base de datos, se usan las migraciones, migraciones es un control de versiones a la base de datos (lo mismo que en Git pero aplicado a la base de datos)
En el contexto de las bases de datos, las migraciones se refieren a un conjunto de archivos o scripts que se utilizan para administrar y controlar los cambios en la estructura de una base de datos a lo largo del tiempo.

> nunca debemos interactuar directamente la bases de datos. por ejemplo usando **SQL** con algún cliente manejador de bases de datos
> 

en caso de querer cambiar datos que ya hemos migrado, agregar un campo, eliminar un campo de alguna tabla, se tiene que hacer con Laravel: 

- **comandos**
    - para crear una migración = `php artisan make:migrate`
    - para ejecutar las migraciones  = `php artisan migrate`
    - para tirar una migración hacia atrás (el ultimo lote)  =  `php artisan migrate:rolback`
- **Schema**
    
    contiene todos los métodos necesarios para poder realizar la creacion de los elementos 
    
    contiene métodos estáticos:
    
    - **créate**: crear una nueva tabla
    - **table**: modificar una tabla existente
    - **dropIfExist**: elimina una tabla si se encuentra en el sistema
- **Blueprint**
    
    es una clase que va contener todo los métodos para generar la estructura de la tabla es decir para generar cada uno de los campos que la tabla va ir necesitando




