# **Control de cambios**

## Fecha de actualización 08-10-19

### Base de datos
```
1. Se modifica el archivo en la carpeta /captura/sql/edca.sql
   a) Se agrega la columna guarantor en la tabla roles.
```

### Sistema de captura
```
1. Se modifica el archivo /captura/views/tabs.ejs

   a) Sección planeación, se ocultan los campos:
    - Fuente de Financiamiento
    - Identificador
    - Denominación de los componentes de la clave presupuestaria
    - Monto
    - Moneda

   b) En la sección ejecución, se elimina el valor "terminated" en el campo implementationstatus.

2. Se modifica el archivo /captura/routes/index.js

   a) Se actualiza el código para la inserción, validación y edición del rol guarantor en la tabla roles.

3. Se modifican los archivos /captura/views/modals/add_party.ejs

   a) Se ordenan los campos en la sección
    Identificador principal:
    - ¿Es persona física?
    Persona moral
    - Nombre o razón social.
    Persona Física
    - Nombre
    - Primer Apellido
    - segundo Apellido

   b) En la sección Papeles del actor:
    - Se agrega el valor "Institución que expide la garantía"

4. Se modifican los archivos /captura/views/modals/edit_party.ejs

   a) Se ordenan los campos en la sección
    Identificador principal:
    - ¿Es persona física?
    Persona moral
    - Nombre o razón social.
    Persona Física
    - Nombre
    - Primer Apellido
    - segundo Apellido

   b) En la sección Papeles del actor:
    - Se agrega el valor "Institución que expide la garantía"
```

## Fecha de actualización 07-11-19

### Base de datos
```
1. Se crean y actualizan los archivos en la carpeta /captura/sql/ para la instalación de la base edca
   a) Se cambia el nombre del archivo edca.sql por schema_edca.sql
   b) Se actualiza el archivo dashboard.sql
   c) Se crea el archivo import_catalogs.sql
   d) Se crea el archivo owner_public.sql
   
2. Se actualiza el archivo db_conf.js para la conexión a la base de datos en la carpeta /captura/

3. Se actualiza el archivo export2Dashboard.js para la conexión a la base de datos en la carpeta /captura/utilities/

4. Se crea el archivo dash_config para la conexión a la base de datos en la carpeta /dashboard/

```

## Fecha de actualización 08-11-19

### Diseño gráfico
```
1. Se actualizan los archivos para el nuevo diseño gráfico 
   a) Se actualiza el header (módulo sistema de captura y dashboard - visualizador)
   b) Se actualiza el footer (módulo sistema de captura y dashboard - visualizador)
   c) Se crea la barra de menú (módulo dashboard - visualizador)

   - Archivos
     1.1 Se agregan las nuevas imágenes necesarias para el header y footer en la carpeta: /captura/public/images/
	 1.2 Se modifica el archivo /captura/public/inai-footer/dgm-footer.html
	 1.3 Se modifica el archivo /captura/public/inai-navbar/dgm-navbar.html
	 1.4 Se modifica el archivo /captura/views/index.ejs
	 1.5 Se agregan las nuevas imágenes necesarias para el header y footer en la carpeta: /dashboard/public/images/
	 1.6 Se modifica el archivo /dashboard/public/inai-footer/dgm-footer.html
	 1.7 Se modifica el archivo /dashboard/public/inai-footer/footer.html
     1.8 Se modifica el archivo /dashboard/public/inai-navbar/dgm-navbar.html
     1.9 Se modifica el archivo /dashboard/public/stylesheets/index.css
     1.10 Se modifica el archivo /dashboard/public/stylesheets/main.css
     1.11 Se modifica el archivo /dashboard/views/acerca.ejs
	 1.12 Se modifica el archivo /dashboard/views/contract.ejs
	 1.13 Se modifica el archivo /dashboard/views/dashboard.ejs
	 1.14 Se crea el archivo /dashboard/views/implementa.ejs
	 1.15 Se modifica el archivo /dashboard/views/index.ejs
	 1.16 Se crea el archivo /dashboard/views/politicadepublicacion.ejs
	 
```