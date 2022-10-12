# phpMyAdmin

## ¿Qué es phpMyAdmin?

phpMyAdmin es una herramienta basada en código PHP que permite administrar bases de datos de MySQL a través del navegador. Esta aplicación está implementada hoy en dia en la mayoría de servidores y hosting compartidos y puedes acceder a ella a través de su panel de control. Página oficial de phpMyAdmin.net.

phpMyAdmin sirve para:

Crear y eliminar Bases de Datos,
Crear, eliminar y alterar  las tablas y campos
Optimizar la base de datos
Ejecutar sentencias SQL
Exportar o Importar la base de datos
Crear una copia de seguridad de la Base de datos

## ¿Cómo acceder a phpMyAdmin?

Puedes acceder al login de phpMyAdmin desde  el panel de control de tu servidor, ya sea un servidor en la nube, un servidor local xampp o similar. Al acceder a phpMyAdmin, puede que te pida loguearte con un usuario y contraseña que tendrás que crear desde el servidor o estará indicada en la información general del servidor.

## Crear una base de datos en phpmyAdmin

Podemos crear nuevas bases de datos desde el panel de control del servidor de manera sencilla pero también las podemos crear una base de datos desde phpMyAdmin si nuestro servidor nos lo permite.

Indicando su nombre y el cotejamiento.

El cotejamiento es el tipo de codificación de la base de datos que permite soportar los tipos de caracteres. Si eres chino utilizaras un cotejamiento de que soporte símbolos chinos.

Normalmente para WordPress será de tipo utf8, por ejemplo, el utf8_spanish_ci es el español moderno que permite tener la ñ en los datos. Y otras como utf8_unicode_ci , utf8_general_ci sirven para guardar datos con caracteres compatibles con muchos idiomas generales.

## Exportar Base de datos

Desde la pestaña Exportar de phpMyAdmin podemos exportar la base de datos para llevarla a otro servidor o para crear una copia de seguridad de la base de datos desde phpMyAdmin.

## Importar la base de datos

Desde la pestaña Importar de phpMyAdmin podemos Importar la base de datos para llevarla a otro servidor o para subirla a otro servidor.

## Ver el tráfico de la base de datos

Sin seleccionar una base de datos, ves a la pestaña Estado Actual, allí puedes encontrar un resumen del tráfico que el servidor de la base de datos a enviado o recibido y las conexiones concurrentes, abortadas y fallidas. Si utilizas un hosting compartido estas cifras puede (seguramente) no sean únicamente las de tu web, si no que serán las de todas las webs que utilicen el mismo servidor.

Pero si es tu servidor te darán unas cifras muy precisas sobre las veces que se consultan las bases de datos y el ancho de banda que consumen.

## Ver las tablas de la base de datos

Si seleccionas una base de datos podrás ver las tablas que la componen y que contienen los datos.
Las tablas de la base de datos por defecto tienen el prefijo wp_ lo puedes cambiar para mejorar la seguridad de tu web. Como cambiar el prefijo de la base de datos de WordPress
Por defecto hay 12 tablas del sistema WordPress pero los plugin de tu web crean sus propias tablas en la base de datos para poder funcionar.
Encontrarás algunas acciones con las que puedes examinar los datos que hay dentro de cada tabla, buscar datos, insertarlos o eliminar una tabla de la base de datos.
También podemos ver cuántas filas hay dentro de cada tabla, el tipo de motor de la base de datos que puede ser InnoDB, MyISAM u otro, el tipo de cotejamiento que es el tipo de codificación de los datos, el tamaño de la tabla y si hay residuos que depurar.

## Optimizar la base de datos

Con las acciones rápidas de la base de datos puedes ejecutar consultas rápidas sobre las tablas, esto es muy útil sobre todo para optimizar la base de datos y limpiarla de espacios en blanco y residuos.

Simplemente selecciona todas las tablas y marca la opción optimizar.

CUIDADO: nada más marcar la opción se ejecuta la consulta seleccionada, si eliges borrar por accidente saldrá un aviso, pero haz una copia de seguridad de la base de datos antes de tocar nada.

## Ver / Editar los datos de una tabla

Si seleccionamos una tabla de WordPress podemos ver los datos alojados en ella.

Por ejemplo en wp_post podrás ver y editar las páginas y entradas del blog de tu web, en wp_comments los comentarios y en wp-users los usuarios.

Esto es realmente útil ya que en ocasiones puedes solucionar ciertos problemas rápidamente si no tienes acceso al panel de control de WordPress, como por ejemplo desde wp_users puedes cambiar la contraseña de un usuario o crear uno nuevo.

También podemos ver las páginas y post y ordenarlos por su ID e incluso editarlos en versión texto plano.

## Borrar tablas de la base de datos

Saber borrar las tablas de una base de datos nos sirve para limpiar la base de datos borrando las tablas de los plugin que ya no tenemos instalados.

Algunos plugin crean tablas en la base de datos para almacenar su configuraciones, pero al desinstalarse pocos plugin autolimpian sus tablas de la base de datos.

Si hemos desinstalado un plugin y sus tablas siguen en la base de datos podemos borrarlas, simplemente selecciona las tablas y pulsa eliminar.