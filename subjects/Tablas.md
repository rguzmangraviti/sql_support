# Crear tablas en phpMyAdmin

## ¿Cómo crear base de datos en PHPMyAdmin?

Primero debemos iniciar sesión en PHPMyAdmin, seleccionar una base de datos donde ingresaremos para generar modificaciones.

Crear una base de datos es muy fácil, la configuración del servidor de tu página podría ser alguno de estos directorios:
//localhost:8888/phpMyAdmin/
//localhost/phpmyadmin
//your_ip_address/phpmyadmin/

Ahí debemos elegir la pestaña “Base de datos”, debemos dar un nombre a la base de datos en el campo “Crear base de datos” y hacer clic en el botón “Crear”.
Debemos confirmar que la base de datos fue correctamente creada al buscarla en la pestaña “Bases de datos”.

## ¿Cómo crear tablas en PHPMyAdmin?

Para la creación de una tabla en una base de datos debemos seleccionar la base de datos correspondiente.
Ahí encontraremos un cuadro donde nos permitirá crear una nueva tabla y debemos colocar un nombre junto con la cantidad de campos dentro de la tabla y haremos clic en el botón “Go”.

Dentro de la nueva tabla podremos incluir los detalles dentro de cada campo.

El primer campo deberá ser “Primary key”, es decir que se completara automáticamente (auto_increment) al agregar entradas nuevas a la tabla, este primer campo deberá llamarse “id” y estará compuesto por un numero entero (Integer) de hasta 4 caracteres de largo.

En el resto de los campos a completar serán campos CHAR (Carácter), debemos asegurarnos que la longitud (length) sea suficiente para ordenar los campos.

Como ejemplo; el segundo campo llevará el nombre name, su tipo será CHAR(esto lo hace un campo donde se guardan números, letras y símbolos) y la longitud será de 100.

Al terminar debemos hacer clic en el botón “Save” y nuestra tabla quedara oficialmente creada.

## Glosario de campos dentro de tabla

Nombre: Nombre de la columna.
Tipo: Tipo de datos que se almacenara en la columna correspondiente.
Valores/longitud: Longitud del campo.
Default: Especificar si los campos de la columna obtienen un valor por defecto.
Colación: Colación de datos para cada campo.
Atributos: Cualquier atributo especial en los campos.
Null: Valor del campo que puede ser null.
Indice: Configura un índice de la fila.
A_i: Abreviatura de incremento automático, si está habilitada, los valores de los campos en la columna se incrementarán automáticamente.
Comentarios: Se podrá añadir un comentario que se incluirá en el código SQL dentro de la base de datos.
