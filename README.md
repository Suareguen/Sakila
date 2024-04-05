# Sakila

Para descargar e instalar la base de datos de ejemplo Sakila en Ubuntu para usarla con MySQL, puedes seguir los siguientes pasos. Asegúrate de tener MySQL instalado en tu sistema antes de comenzar.

Descargar el Archivo de Sakila:
Abre una terminal y utiliza wget para descargar los archivos necesarios de Sakila desde el repositorio oficial de MySQL.
```
wget https://downloads.mysql.com/docs/sakila-db.tar.gz
```
Extraer el Archivo Descargado:
Una vez descargado, debes extraer el contenido del archivo .tar.gz.

```
tar -xzvf sakila-db.tar.gz
```
Acceder al Directorio de Sakila:
Cambia al directorio que contiene los archivos de Sakila.

```
cd sakila-db
```

Iniciar Sesión en MySQL:
Ahora, inicia sesión en tu servidor MySQL como root o como un usuario que tenga privilegios suficientes para crear bases de datos y manipular privilegios.

```
mysql -u user -p
```

Te pedirá la contraseña del usuario root de MySQL.

Crear la Base de Datos Sakila y Cargar la Estructura:
Dentro de la interfaz de comandos de MySQL, primero crea la base de datos Sakila y luego carga el esquema de la base de datos desde el archivo sakila-schema.sql.

```
CREATE DATABASE sakila;
USE sakila;
SOURCE sakila-schema.sql;
```

Cargar los Datos de Sakila:
Después de haber cargado el esquema, el siguiente paso es cargar los datos en sí mismos desde el archivo sakila-data.sql.

```
SOURCE sakila-data.sql;
```
