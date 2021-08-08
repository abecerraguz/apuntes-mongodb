# Apuntes de Mongo DB

![MongoDB](mongodb-install-1536x1152.jpeg)


## Debemos instalar 

Ejecute la terminal y luego escriba `brew tap mongodb/brew`, luego `brew install mongodb-community@5.0`

## Ejecutando el servidor MongoDB

Escriba en la terminal `brew services start mongodb-community`

Eso es. Si eso fue exitoso, el terminal debería llenarse con un montón de información y no debería poder ver la línea de aviso normal del terminal, solo un subrayado. Esto significa que su servidor está en funcionamiento. Lo que hemos hecho es ejecutar nuestro servidor de base de datos y, por lo tanto, abrir nuestras bases de datos MongoDB para conexiones, de modo que podamos consultar la base de datos y realizar operaciones CRUD.



## Conéctese a su base de datos:

Para conectarse a sus bases de datos MongoDB, en su terminal, escriba ...

```bash

mongo

```
Ahora debería ver que el cursor del terminal se convierte en una sola flecha y un pitido subrayado.

## Iniciar y detener el proceso:

Para ejecutar MongoDB (es decir, el mongodproceso) manualmente como un proceso en segundo plano , ejecute:

```bash

brew services start mongodb-community@5.0

```

```bash

brew services stop mongodb-community@5.0

```
## Organización de Mongo DB

Pimero tenemos un `Cluster`, que es como mi computadora, dentro del cluster tenemos `colecciones`, dentro de las colecciones tenemos bases de datos que a su ves la base de datos esta compuesta por documentos que en su globalidad conforman una colección.


## RESUMEN:

Iniciar el proceso de Mongo `brew services start mongodb-community@5.0`
Conectarse a sus bases de datos `mongo`
Para salir de `mongo` puedes escribir `exit`
Para mostrar Bases de datos `show dbs`
Para crear una base de datos `use nombre_base_datos`
Para crear una coleccion `db.createCollection('usuarios')`
Para saber donde estoy o en que base de datos `db`
Para insertar un dato en usuarios `db.usuarios.insertOne({name:'juan'})`
Para mostrar todos los documentos de la colección `db.usuarios.find()`

    



