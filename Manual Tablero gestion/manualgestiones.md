
![badge](imagenes/badge.webp)

# Manual Reporte Gestores

## Indice

- [Manual Reporte Gestores](#manual-reporte-gestores)
   -[Indice](#indice)
  - [1.ALIADOS DE TRABAJO Y HERRAMIENTAS](#1-aliados-de-trabajo-y-herramientas)
  - [Commit 2. Inicio Web Service Turbot](#commit-2-inicio-web-service-turbot)
  - [Commit 3. Cargue del Loggin](#commit-3-cargue-del-loggin)
  - [Commit 4. Actualización vista administrador (relational data bases)](#commit-4-actualización-vista-administrador-relational-data-bases)
    - [Clase 4 Entidades y atributos](#clase-4-entidades-y-atributos)
      - [Atributos](#atributos)
      - [Entidades](#entidades)
      - [Clase 5 Entidades de Platzi Blog](#clase-5-entidades-de-platzi-blog)
    - [Clase 6 Relaciones](#clase-6-relaciones)
      - [Cardinalidad: 1 a 1](#cardinalidad-1-a-1)
      - [Cardinalidad: 0 a 1](#cardinalidad-0-a-1)
      - [Cardinalidad: 1 a N (1 a muchos)](#cardinalidad-1-a-n-1-a-muchos)
      - [Cardinalidad: 0 a N](#cardinalidad-0-a-n)
    - [Clase 7 Multiples muchos](#clase-7-multiples-muchos)
    - [Clase 8 Diagrama ER](#clase-8-diagrama-er)
    - [Clase 9 Diagrama Físico: tipos de datos y constraints](#clase-9-diagrama-físico-tipos-de-datos-y-constraints)
      - [Tipos de dato](#tipos-de-dato)
      - [Constraints (Restricciones)](#constraints-restricciones)
    - [Clase 10 Diagrama Físico: normalizacion](#clase-10-diagrama-físico-normalizacion)
    - [Clase 11 Diagrama Físico: normalizando Platziblog](#clase-11-diagrama-físico-normalizando-platziblog)
      - [Diagram Entidad Relacion](#diagram-entidad-relacion)
      - [Diagrama fisico Paso 1](#diagrama-fisico-paso-1)
      - [Diagrama fisico Paso 2](#diagrama-fisico-paso-2)
      - [Diagrama fisico Paso 3](#diagrama-fisico-paso-3)
    - [Clase 12 Formas normales en DB relacionales](#clase-12-formas-normales-en-db-relacionales)
      - [Primera Forma Normal (1FN)](#primera-forma-normal-1fn)
      - [Segunda Forma Normal (2FN)](#segunda-forma-normal-2fn)
      - [Tercera Forma Normal (3FN)](#tercera-forma-normal-3fn)
      - [Cuarta Forma Normal (4FN)](#cuarta-forma-normal-4fn)
  - [Modulo 3 RDBMS (MySQL) o cómo hacer lo anterior de manera práctica](#modulo-3-rdbms-mysql-o-cómo-hacer-lo-anterior-de-manera-práctica)
    - [Clase 13 RDB Qué](#clase-13-rdb-qué)
    - [Clase 14 Instalación local de un RDBMS (Windows)](#clase-14-instalación-local-de-un-rdbms-windows)
    - [Clase 15  Instalación local de un RDBMS (Mac)](#clase-15--instalación-local-de-un-rdbms-mac)
    - [Clase 16 Instalación local de un RDBMS (Ubuntu)](#clase-16-instalación-local-de-un-rdbms-ubuntu)
    - [Clase 17 Clientes Graficos](#clase-17-clientes-graficos)
    - [Clase 18 Servicios administrados](#clase-18-servicios-administrados)
  - [Modulo 4 SQL hasta en la sopa](#modulo-4-sql-hasta-en-la-sopa)
    - [Clase 19 Historia de SQL](#clase-19-historia-de-sql)
    - [Clase 20 DDL create](#clase-20-ddl-create)
    - [Clase 21 CREATE VIEW y DDL ALTER](#clase-21-create-view-y-ddl-alter)
      - [Create view](#create-view)
      - [Alter Table](#alter-table)
      - [Drop Column Borrando una columna](#drop-column-borrando-una-columna)
    - [Clase 22 DDL drop](#clase-22-ddl-drop)
    - [Clase 23 DML](#clase-23-dml)
      - [Insert](#insert)
      - [Update](#update)
      - [Delete](#delete)
      - [Select](#select)
    - [Clase 24 Que tan standard es SQL](#clase-24-que-tan-standard-es-sql)
    - [Clase 25 Creando Platziblog: tablas independientes](#clase-25-creando-platziblog-tablas-independientes)
    - [Clase 26 Creando Platziblog: tablas transitivas](#clase-26-creando-platziblog-tablas-transitivas)
    - [Clase 27 Creando Platziblog: tablas transitivas](#clase-27-creando-platziblog-tablas-transitivas)
      - [Reverse Engineer](#reverse-engineer)
    - [Clase 28 Por qué las consultas son tan importantes](#clase-28-por-qué-las-consultas-son-tan-importantes)
    - [Clase 29 Estructura básica de un Query](#clase-29-estructura-básica-de-un-query)
      - [Primer Consulta](#primer-consulta)
    - [Clase 30 SELECT](#clase-30-select)
    - [Clase 31 FROM](#clase-31-from)
    - [Clase 32 Utilizando la sentencia FROM](#clase-32-utilizando-la-sentencia-from)
    - [Clase 33 WHERE](#clase-33-where)
    - [Clase 34 Utilizando la sentencia WHERE nulo y no nulo](#clase-34-utilizando-la-sentencia-where-nulo-y-no-nulo)
    - [Clase 35 GROUP BY](#clase-35-group-by)
    - [Clase 36 ORDER BY y HAVING](#clase-36-order-by-y-having)
    - [Clase 37 El interminable agujero de conejo (Nested queries)](#clase-37-el-interminable-agujero-de-conejo-nested-queries)
    - [Clase 38 Como convertir una pregunta en un query SQL](#clase-38-como-convertir-una-pregunta-en-un-query-sql)
      - [De pregunta a Query](#de-pregunta-a-query)
    - [Clase 39 Preguntandole a la base de datos](#clase-39-preguntandole-a-la-base-de-datos)
    - [Clase 40 Consultando PlatziBlog](#clase-40-consultando-platziblog)
  - [Modulo 4 Introduccion a la bases de datos NO relacionales](#modulo-4-introduccion-a-la-bases-de-datos-no-relacionales)
    - [Clase 41 Que son y cuales son los tipos de bases de datos no relacionales](#clase-41-que-son-y-cuales-son-los-tipos-de-bases-de-datos-no-relacionales)
      - [Tipos de bases de datos no relacionales:](#tipos-de-bases-de-datos-no-relacionales)
    - [Clase 42 Servicios administrados y jerarquía de datos](#clase-42-servicios-administrados-y-jerarquía-de-datos)
  - [Modulo 5 Manejo de modelos de datos en bases de datos no relacionales](#modulo-5-manejo-de-modelos-de-datos-en-bases-de-datos-no-relacionales)
    - [Clase 43 Top level collection con Firebase](#clase-43-top-level-collection-con-firebase)
    - [Clase 44 Creando y borrando documentos en Firestore](#clase-44-creando-y-borrando-documentos-en-firestore)
    - [Clase 45 Colecciones vs subcolecciones](#clase-45-colecciones-vs-subcolecciones)
    - [Clase 46 Recreando Platziblog](#clase-46-recreando-platziblog)
    - [Clase 47 Construyendo Platziblog en Firestore](#clase-47-construyendo-platziblog-en-firestore)
    - [Clase 48 Proyecto final: transformando tu proyecto en una db no relacional](#clase-48-proyecto-final-transformando-tu-proyecto-en-una-db-no-relacional)
      - [Regla 1. Piensa en la vista de tu aplicación](#regla-1-piensa-en-la-vista-de-tu-aplicación)
  - [Modulo 6 Bases de datos en la vida real](#modulo-6-bases-de-datos-en-la-vida-real)
    - [Clase 49 Bases de datos en la vida real](#clase-49-bases-de-datos-en-la-vida-real)
    - [Clase 50 Big Data](#clase-50-big-data)
    - [Clase 51 Data warehouse](#clase-51-data-warehouse)
    - [Clase 52 Data mining](#clase-52-data-mining)
    - [Clase 53 ETL](#clase-53-etl)
    - [Clase 54 Business intelligence](#clase-54-business-intelligence)
    - [Clase 55 Machine Learning](#clase-55-machine-learning)
    - [Clase 56 Data Science](#clase-56-data-science)
    - [Clase 57 Por que aprender bases de datos hoy](#clase-57-por-que-aprender-bases-de-datos-hoy)
  - [Bonus](#bonus)
    - [Clase 58 Bases de datos relacionales vs no relacionales](#clase-58-bases-de-datos-relacionales-vs-no-relacionales)

## 1. ALIADOS DE TRABAJO Y HERRAMIENTAS

![imagenes/aliadosyherramientas.PNG](imagenes/aliadosyherramientas.PNG)

## Q 2. ALIADOS DE TRABAJO Y HERRAMIENTAS

Creación de la estructura que usaremeos en nuestro web service, se decide usar para HTML y CSS Bootstrap que es un framework front-end utilizado para desarrollar aplicaciones web ya que agiliza el diseño al contar con variación de plantillas y complementos para JavaScript tambien se opta por manejar Django es un framework de desarrollo web de código abierto, escrito en Python, que respeta el patrón de diseño conocido como modelo–vista–controlador y nos ayudara a cómo configurar un entorno de desarrollo y cómo empezar a usarlo para crear tus propias aplicaciones web. Por ultimo como gestor de bases relacionales utilizaremos PostgreSQL. 

## Commit 3. Cargue del Loggin

Se genera la creacion de la vista principal del loggin donde los usuarios finales ingresaran sus datos y este realizara una validacion de credenciales para poder dar acceso a la pagina inicialmente antes de crear la conexión a la base y proceder a configurar las validaciones, se realiza un diseño de estilos para poder volver el front más amigable a los usuarios, se decide tomar la paleta de colores DataPro

![src/loggin.PNG](src/loggin.PNG)

## Commit 4. Actualización vista administrador (relational data bases)

![image](https://user-images.githubusercontent.com/114417877/196577914-49c6a91d-2f7f-4d34-8aca-15ce078e458f.png)

### Clase 4 Entidades y atributos

Una **entidad** es algo similar a un objeto (programación orientada a objetos) y representa algo en el mundo real, incluso algo abstracto. Tienen atributos que son las cosas que los hacen ser una entidad, se diagraman dentro de cuadrados  y **por convención se ponen en plural**.

#### Atributos

Los atributos se representan con óvalos, los que tienen multiples valores llevan dobles óvalos, también existen atributos compuestos, los atributos especiales son óvalos con linea punteada.

Los **atributos compuestos** son aquellos que tienen atributos ellos mismos.

Los **atributos llave** son aquellos que identifican a la entidad y no pueden ser repetidos, se diagraman con underline. Existen:

- Naturales: Son inherentes al objeto como el número de serie
- Clave artificial: No es inherente al objeto y se asigna de manera arbitraria

![src/Atributos-rdb.png](src/Atributos-rdb.png)

#### Entidades

**Entidad Fuerte:** No depende de ninguna entidad para existir

**Entidades débiles:** No pueden existir sin una entidad fuerte y se representan con un cuadrado con doble línea.

- Identidades débiles por identidad: No se diferencian entre sí más que por la clave de su identidad fuerte.
- Identidades débiles por existencia: Se les asigna una clave propia.

![src/entidades_debiles.png](src/entidades_debiles.png)

![src/entidades_debiles_2.png](src/entidades_debiles_2.png)

Las entidades debiles pueden serlo por dos motivos:

**Por identidad:** No se diferencian entre si mas que por la clave de su entidad fuerte (clave isbn).

**Por existencia:** Usando llave asignada por nosotros (un id).

#### Clase 5 Entidades de Platzi Blog

Nuestro proyecto será un manejador de Blogpost. Es un contexto familiar y nos representará retos muy interesantes.

- Primer paso: Identificar las entidades (abstracciones del mundo real).

![src/entidades_platziblog.png](src/entidades_platziblog.png)

- Segundo paso: Pensar en los atributos.

![src/entidades_platziblog_2.png](src/entidades_platziblog_2.png)

![src/entidades_platziblog_3.png](src/entidades_platziblog_3.png)

### Clase 6 Relaciones

Las **relaciones** nos permiten ligar o unir nuestras diferentes entidades y se representan con rombos. Por convención se definen a través de verbos.

![src/relaciones.png](src/relaciones.png)

Las relaciones tienen una propiedad llamada **cardinalidad** y tiene que ver con números. Cuántos de un lado pertenecen a cuántos del otro lado:

Cardinalidad: 1 a 1
Cardinalidad: 0 a 1
Cardinalidad: 1 a N
Cardinalidad: 0 a N

#### Cardinalidad: 1 a 1

![src/cardinalidad_1_1.png](src/cardinalidad_1_1.png)

1 persona - tiene - 1 dato_contacto
1 dato_contacto - tiene - 1 persona.

#### Cardinalidad: 0 a 1

Algunos autores la denominan 1 a 1 opcional.
En el ejemplo una sesión tiene un usuario, pero no necesariamente esta loggeado todo  el tiempo

![src/cardinalidad_0_1.png](src/cardinalidad_0_1.png)

#### Cardinalidad: 1 a N (1 a muchos)

Un automóvil tiene N automóviles, pero 1 automóvil solo tiene 1 dueño.

![src/cardinalidad_1_N.png](src/cardinalidad_1_N.png)

#### Cardinalidad: 0 a N

![src/33333333333333333333333333333333333333333333333333333333333333333333.png](src/cardinalidad_0_N.png)

### Clase 7 Multiples muchos

Este tipo de cardinalidad es muy interesante por ello su clase aparte,se vera cuando veamos los campos clave.

Cardinalidad: N a N

### Clase 8 Diagrama ER

Un diagrama es como un mapa y nos ayuda a entender cuáles son las entidades con las que vamos a trabajar, cuáles son sus relaciones y qué papel van a jugar en las aplicaciones de la base de datos.

![src/diagrama_ER.png](src/diagrama_ER.png)

### Clase 9 Diagrama Físico: tipos de datos y constraints

Para llevar a la práctica un diagrama debemos ir más allá y darle detalle con parámetros como:

#### Tipos de dato

**- Texto:** CHAR(n), VARCHAR(n), TEXT
**- Números:** INTEGER, BIGINT, SMALLINT, DECIMAL(n,s), NUMERIC(n,s)
**- Fecha/hora:** DATE, TIME, DATETIME, TIMESTAMP
**- Lógicos:** BOOLEAN

Nota:

Char(8) reserva 8 espacios en memoria de forma fija, Varchar(8) hace lo mismo pero crece (1,2,3...8) de manera dinámica conforme los requieres y tiene un limite general de 255 caracteres.

#### Constraints (Restricciones)

**- NOT NULL:** Se asegura que la columna no tenga valores nulos
**- UNIQUE:** Se asegura que cada valor en la columna no se repita
**- PRIMARY KEY:** Es una combinación de NOT NULL y UNIQUE
**- FOREIGN KEY:** Identifica de manera única una tupla en otra tabla
**- CHECK:** Se asegura que el valor en la columna cumpla una condición dada
**- DEFAULT:** Coloca un valor por defecto cuando no hay un valor especificado
**- INDEX:** Se crea por columna para permitir búsquedas más rápidas, tiene la desventaja de que tiene que reindexar los registros cada vez, lo que vuelve muy lenta la operación de la bd.

### Clase 10 Diagrama Físico: normalizacion

La normalización como su nombre lo indica nos ayuda a dejar todo de una forma normal. Esto obedece a las 12 reglas de Codd y nos permiten separar componentes en la base de datos:

**Primera forma normal (1FN):** Atributos atómicos (Sin campos repetidos)
**Segunda forma normal (2FN):** Cumple 1FN y cada campo de la tabla debe depender de una clave única.
**Tercera forma normal (3FN):** Cumple 1FN y 2FN y los campos que NO son clave, NO deben tener dependencias.
**Cuarta forma normal (4FN):** Cumple 1FN, 2FN, 3FN y los campos multivaluados se identifican por una clave única.

![src/diagrama_fisico_sin_normalizar.png](src/diagrama_fisico_sin_normalizar.png)

**Primera forma normal (1FN):** Atributos atómicos (Sin campos repetidos)

![src/diagrama_fisico_1N.png](src/diagrama_fisico_1N.png)

**Segunda forma normal (2FN):** Cumple 1FN y cada campo de la tabla debe depender de una clave única.

![src/diagrama_fisico_2N.png](src/diagrama_fisico_2N.png)

**Tercera forma normal (3FN):** Cumple 1FN y 2FN y los campos que NO son clave, NO deben tener dependencias.

![src/diagrama_fisico_3N.png](src/diagrama_fisico_3N.png)

**Cuarta forma normal (4FN):** Cumple 1FN, 2FN, 3FN y los campos multivaluados se identifican por una clave única.

![src/diagrama_fisico_4N.png](src/diagrama_fisico_4N.png)

### Clase 11 Diagrama Físico: normalizando Platziblog

#### Diagram Entidad Relacion

![src/diagrama_ER.png](src/diagrama_ER.png)

#### Diagrama fisico Paso 1

Generar los campos básicos de cada entidad

![src/Diagrama_Fisico_paso_1.png](src/Diagrama_Fisico_paso_1.png)

#### Diagrama fisico Paso 2

Genera las relaciones entre cada entidad y asigna PK y FK.

![src/diagrama_fisico_paso_2.png](src/diagrama_fisico_paso_2.png)

#### Diagrama fisico Paso 3

![src/diagrama_fisico_paso_2_N_N.png](src/diagrama_fisico_paso_2_N_N.png)

Para manejar las relaciones muchos a muchos, es necesario generar una tabla intermedia de esta manera.

![src/diagrama_fisico_paso_3_N_N.png](src/diagrama_fisico_paso_3_N_N.png)

Observa que post_id y etiqueta_id usan llaves compuestas para hacer combinaciones únicas, o podemos generar también la forma anterior con un id

### Clase 12 Formas normales en DB relacionales

La normalización en las bases de datos relacionales es uno de esos temas que, por un lado es sumamente importante y por el otro suena algo esotérico. Vamos a tratar de entender las formas normales (FN) de una manera simple para que puedas aplicarlas en tus proyectos profesionales.

#### Primera Forma Normal (1FN)

Esta FN nos ayuda a eliminar los valores repetidos y no atómicos dentro de una base de datos.

Formalmente, una tabla está en primera forma normal si:

- Todos los atributos son atómicos. Un atributo es atómico si los elementos del dominio son simples e indivisibles.
- No debe existir variación en el número de columnas.
- Los campos no clave deben identificarse por la clave (dependencia funcional).
- Debe existir una independencia del orden tanto de las filas como de las columnas; es decir, si los datos cambian de orden no deben cambiar sus significados.

Se traduce básicamente a que si tenemos campos compuestos como por ejemplo “nombre_completo” que en realidad contiene varios datos distintos, en este caso podría ser “nombre”, “apellido_paterno”, “apellido_materno”, etc.

Se traduce básicamente a que si tenemos campos compuestos como por ejemplo “nombre_completo” que en realidad contiene varios datos distintos, en este caso podría ser “nombre”, “apellido_paterno”, “apellido_materno”, etc.

Los campos deben ser tales que si reordenamos los registros o reordenamos las columnas, cada dato no pierda el significado.

#### Segunda Forma Normal (2FN)

Esta FN nos ayuda a diferenciar los datos en diversas entidades.

Formalmente, una tabla está en segunda forma normal si:

- Está en 1FN
- Sí los atributos que no forman parte de ninguna clave dependen de forma completa de la clave principal. Es decir, que no existen dependencias parciales.
- Todos los atributos que no son clave principal deben depender únicamente de la clave principal.

Lo anterior quiere decir que sí tenemos datos que pertenecen a diversas entidades, cada entidad debe tener un campo clave separado. Por ejemplo:

![diagrama_fisico_1N.png](src/diagrama_fisico_1N.png)

En la tabla anterior tenemos por lo menos dos entidades que debemos separar para que cada uno dependa de manera única de su campo llave o ID. En este caso las entidades son alumnos por un lado y materias por el otro, ya que una materia. En el ejemplo anterior, quedaría de la siguiente manera:

![diagrama_fisico_2N.png](src/diagrama_fisico_2N.png)

#### Tercera Forma Normal (3FN)

Esta FN nos ayuda a separar conceptualmente las entidades que no son dependientes.

Formalmente, una tabla está en tercera forma normal si:

Se encuentra en 2FN
No existe ninguna dependencia funcional transitiva en los atributos que no son clave

Esta FN se traduce en que aquellos datos que no pertenecen a la entidad deben tener una independencia de las demás y debe tener un campo clave propio. Continuando con el ejemplo anterior, al aplicar la 3FN separamos la tabla alumnos ya que contiene datos de los cursos en ella quedando de la siguiente manera.

![diagrama_fisico_3N.png](src/diagrama_fisico_3N.png)

#### Cuarta Forma Normal (4FN)

Esta FN nos **trata de atomizar los datos multivaluados** de manera que no tengamos datos repetidos entre rows.

Formalmente, una tabla está en cuarta forma normal si:

- Se encuentra en 3FN
- Los campos multivaluados se identifican por una clave única

Esta FN trata de eliminar registros duplicados en una entidad, es decir que cada registro tenga un contenido único y de necesitar repetir la data en los resultados se realiza a través de claves foráneas.

Aplicado al ejemplo anterior la tabla materia se independiza y se relaciona con el alumno a través de una tabla transitiva o pivote, de tal manera que si cambiamos el nombre de la materia solamente hay que cambiarla una vez y se propagara a cualquier referencia que haya de ella.

![diagrama_fisico_4N](src/diagrama_fisico_4N.png)

De esta manera, aunque parezca que la información se multiplicó, en realidad la descompusimos o normalizamos de manera que a un sistema le sea fácil de reconocer y mantener la consistencia de los datos.

Algunos autores precisan una 5FN que hace referencia a que después de realizar esta normalización a través de uniones (JOIN) permita regresar a la data original de la cual partió.

## Modulo 3 RDBMS (MySQL) o cómo hacer lo anterior de manera práctica

### Clase 13 RDB Qué

**RDBMS** significa Relational Database Management System o sistema manejador de bases de datos relacionales. Es un programa que se encarga de seguir las reglas de Codd y se puede utilizar de manera programática.

### Clase 14 Instalación local de un RDBMS (Windows)

Hay dos maneras de acceder a manejadores de bases de datos:

- Instalar en máquina local un administrador de bases relacional.
-Tener ambientes de desarrollo especiales o servicios cloud.

En este curso usaremos MySQL porque tiene un impacto histórico siendo muy utilizado y además es software libre y gratuito. La versión 5.6.43 es compatible con la mayoría de aplicaciones y frameworks.

- Root es el usuario principal que tendrá todos los permisos y por lo tanto en ambientes de producción hay que tener mucho cuidado al configurarlo.

Link
<https://dev.mysql.com/downloads/windows/installer/5.6.html>

Procedimiento:

- Descargamos e instalamos como es usual en windows
- En el instalador seleccionamos la opción custom
- Instalamos MySQL Server la version 64bts
- Instalamos MySQL Workbench (ignoramos lo demás)

![Instalador_mysql_1](src/Instalador_mysql_1.png)
![Instalador_mysql_2](src/Instalador_mysql_2.png)
![Instalador_mysql_3](src/Instalador_mysql_3.png)

### Clase 15  Instalación local de un RDBMS (Mac)

La instalación es similar al todos los instaladores en mac, descarga el archivo .dmg

<https://dev.mysql.com/downloads/workbench/>

Para macOS debes descargar workbench aparte.

<https://dev.mysql.com/downloads/mysql/5.7.html>

### Clase 16 Instalación local de un RDBMS (Ubuntu)

Visita la dirección de descarga de la versión de comunidad de MySql
<https://dev.mysql.com/downloads/mysql/5.7.html#downloads>

Dirígete a la sección de selección de descargas y selecciona tu distribución de Linux. En nuestro caso Ubuntu y selecciona posteriormente la versión que estás utilizando actualmente, en nuestro caso 18.04 de 64 bits.

Los pasos son similares a los otros sistemas, descarga el paquete .deb, también puedes instalar desde la consola

sudo apt-get install mysql-server

### Clase 17 Clientes Graficos

Observamos el preview y pasos para crear un schema en Mysql workbench

![worckbench_1](src/worckbench_1.png)

![worckbench_2](src/worckbench_2.png)

![worckbench_3](src/worckbench_3.png)

### Clase 18 Servicios administrados

Hoy en día muchas empresas ya no tienen instalados en sus servidores los RDBMS sino que los contratan a otras personas. Estos servicios administrados cloud te permiten concentrarte en la base de datos y no en su administración y actualización.

Introducción a google cloud, toma el curso para configurarlo.

## Modulo 4 SQL hasta en la sopa

### Clase 19 Historia de SQL

**SQL** significa Structured Query Language y tiene una estructura clara y fija. Su objetivo es hacer un solo lenguaje para consultar cualquier manejador de bases de datos volviéndose un gran estándar.

Ahora existe el **NOSQL** o Not Only Structured Query Language que significa que no sólo se utiliza SQLen las bases de datos no relacionales.

### Clase 20 DDL create

SQL tiene dos grandes sublenguajes:

**DDL o Data Definition Language** que nos ayuda a crear la estructura de una base de datos. Existen 3 grandes comandos:

**- Create**: Nos ayuda a crear bases de datos, tablas, vistas, índices, etc.

-**Alter**: Ayuda a alterar o modificar entidades.

**- Drop**: Nos ayuda a borrar. Hay que tener cuidado al utilizarlo.

**3 objetos que manipularemos con el lenguaje DDL:**

- Database o bases de datos
- Table o tablas. Son la traducción a SQL de las entidades
- View o vistas: Se ofrece la proyección de los datos de la base de datos de forma entendible.

![SQL_create_database](src/SQL_create.png)

![SQL_create](src/SQL_create_database.png)

Seleccionamos el schema  como default, de forma gráfica aunque con la terminal seria el use database.

![worckbench_default_schema.png](src/worckbench_default_schema.png)

El comando Create Table

![create_table_slide](src/create_table_slide.png)

El creamos con workbench la tabla anterior, definimos  cada uno de los campos de manera sencilla posterior damos apply

![worckbench_new_table_1.png](src/worckbench_new_table_1.png)

![worckbench_new_table_2_apply.png](src/worckbench_new_table_2_apply.png)

![worckbench_new_table_3.png](src/worckbench_new_table_3.png)

### Clase 21 CREATE VIEW y DDL ALTER

#### Create view

![workbench_create_view.png](src/workbench_create_view.png)

Para iniciar el ejercicio insertamos datos en la BD,  copiamos la sentencia
`SELECT * FROM platziblog.people;`, nos movemos a views y damos click derecho y create view.

Views ya cuenta con la parte inicial de la sentencia de create view, pegamos debajo el select y damos apply

```mysql
CREATE VIEW 'new_view' AS
SELECT * FROM platziblog.people;
```

![create_view1](src/create_view1.png)

![create_view2](src/create_view2.png)

![create_view3](src/create_view3.png)

![create_view4](src/create_view4.png)

Parece redundante la información, pero podemos estructurar las consultas junto con otras tablas, y estas vistas mantendrán la consulta sin necesidad de acer la de nuevo incrementando los  datos de forma automática.

#### Alter Table

!![alter_table_1](src/alter_table_1.png)

!![alter_table_2](src/alter_table_2.png)

!![alter_table_3](src/alter_table_3.png)

!![alter_table_4](src/alter_table_4.png)

!![alter_table_1](src/alter_table_1.png)

#### Drop Column Borrando una columna

Click derecho y deled selected

!![drop_column_1](src/drop_column_1.png)

!![drop_column_1](src/drop_column_2.png)

### Clase 22 DDL drop

Está puede ser la sentencia ¡más peligrosa! (????), sobre todo cuando somos principiantes. Básicamente borra o desaparece de nuestra base de datos algún elemento.

Pasos para borrar una tabla

![drop_table](src/drop_table.png)

![drop_table_1](src/drop_table_1.png)

![drop_table_2](src/drop_table_2.png)

![drop_table_3](src/drop_table_3.png)

Pasos para borrar la base de datos o schema

![drop_schema_1](src/drop_schema_1.png)

![drop_schema_2](src/drop_schema_2.png)

![drop_schema_3](src/drop_schema_3.png)

![drop_schema_4](src/drop_schema_4.png)

Nota: las herramientas del DDL se utilizan mayormente en la fase de construcción y mantenimiento de las bases de datos, la manipulación u operación se hace con DML.

### Clase 23 DML

**DML** trata del contenido de la base de datos. Son las siglas de Data Manipulation Language y sus comandos son:

**- Insert:** Inserta o agrega nuevos registros a la tabla.
**- Update:** Actualiza o modifica los datos que ya existen.
**- Delete:** Esta sentencia es riesgosa porque puede borrar el contenido de una tabla.
**- Select:** Trae información de la base de datos.

#### Insert

Crearemos este comando en una BD nueva llamada platzi_test con la con la estructura del ejercicio anterior

![insert_command.png](src/insert_command.png)

En la seccion de query realizamos el comando

```sql
INSERT INTO people(last_name, first_name, address, city)
VALUES ('Hernandez', 'Laura', 'Calle 21', 'Monterrey');
```

Insertamos los valores con el símbolo de rayo o con ctrl + enter

![insert_command_1.png](src/insert_command_1.png)

![insert_command_2.png](src/insert_command_2.png)

#### Update

![update_command.png](src/update_command.png)

comandos

```sql
UPDATE people SET last_name = 'Chavez', city = 'Merida'
WHERE person_id = 1;
```

![update_command_1.png](src/update_command_1.png)

![update_command_2.png](src/update_command_2.png)

#### Delete

```sql
DELETE FROM people WHERE person_id = 1;
```

![delete__command_1.png](src/delete__command_1.png)

#### Select

![select_command.png](src/select_command.png)

```sql
SELECT first_name, last_name FROM people;
```

![select_command_1.png](src/select_command_1.png)

### Clase 24 Que tan standard es SQL

La utilidad más grande de SQL fue unificar la forma en la que pensamos y hacemos preguntas a un repositorio de datos. Ahora que nacen nuevas bases de datos igualmente siguen tomando elementos de SQL.

Practicamos lo anterior como repaso.

```sql
CREATE TABLE people(
person_id int,
last_name VARCHAR(255),
first_name VARCHAR(255),
address VARCHAR(255),
city VARCHAR(255)
);

INSERT INTO people (last_name, first_name, address, city)
VALUES (‘Hernandez’, ‘Laura’, ‘Calle 21’, ‘Monterrey’);
.

SELECT first_name, last_name FROM people;


DROP TABLE people;
```

Realizamos  lo  mismo en una instancia de postgre gcloud

Tal cual pegamos crear tabla

```sql
CREATE TABLE people(
person_id int,
last_name VARCHAR(255),
first_name VARCHAR(255),
address VARCHAR(255),
city VARCHAR(255)
);
```

revisamos las tablas con

```sql
\dt
```

Hacemos las operaciones anteriores

```sql

INSERT INTO people (last_name, first_name, address, city)
VALUES (‘Hernandez’, ‘Laura’, ‘Calle 21’, ‘Monterrey’);
.

SELECT first_name, last_name FROM people;


DROP TABLE people;
```

El DDL y DML en ambos  motores de bases de datos es estandar, cambian solo funciones internas.

### Clase 25 Creando Platziblog: tablas independientes

- Una buena práctica es comenzar creando las entidades que no tienen una llave foránea.
- Generalmente en los nombres de bases de datos se evita usar eñes o acentos para evitar problemas en los manejadores de las bases de datos.

![diagrama_fisico_paso_2](src/diagrama_fisico_paso_2.png)

Creamos el schema `platziblog` y seleccionamos como default y creamos las siguientes tablas

- categorías
  
![platziblog_tabla_etiquetas_1](src/platziblog_tabla_caracteristicas_1.png)

![platziblog_tabla_caracteristicas_2](src/platziblog_tabla_caracteristicas_2.png)

Creamos de igual forma la tabla Etiquetas

![platziblog_tabla_etiquetas_1](src/platziblog_tabla_etiquetas_1.png)

![platziblog_tabla_etiquetas_2](src/platziblog_tabla_etiquetas_2.png)

Tabla Usuarios

![platziblog_tabla_usuarios_1.png](src/platziblog_tabla_usuarios_1.png)

![platziblog_tabla_usuarios_2.png](src/platziblog_tabla_usuarios_2.png)

### Clase 26 Creando Platziblog: tablas transitivas

Creando Platziblog: tablas dependientes
El comando **“cascade”** sirve para que cada que se haga un update en la tabla principal, se refleje también en la tabla en la que estamos creando la relación.

![platziblog_tabla_post_1.png](src/platziblog_tabla_post_1.png)

![platziblog_tabla_post_2.png](src/platziblog_tabla_post_2.png)

Vamos a la pestaña Foreign Key y asignamos las relaciones.

Asignamos la llave foranea del usuario_id

![platziblog_tabla_post_fk_usuario_id.png](src/platziblog_tabla_post_fk_usuario_id.png)

![platziblog_tabla_post_fk_categorias_id.png](src/platziblog_tabla_post_fk_categorias_id.png)

![platziblog_tabla_post_fk_categorias_id_1.png](src/platziblog_tabla_post_fk_categorias_id_1.png)

### Clase 27 Creando Platziblog: tablas transitivas

- Las tablas transitivas sirven como puente para unir dos tablas. No tienen contenido semántico.

- **Reverse Engineer** nos reproduce el esquema del cual nos basamos para crear nuestras tablas. Es útil cuando llegas a un nuevo trabajo y quieres entender cuál fue la mentalidad que tuvieron al momento de crear las bases de datos.

Creamos la tabla comentarios.

![platziblog_tabla_comentarios.png](src/platziblog_tabla_comentarios.png)

![platziblog_tabla_comentarios_1.png](src/platziblog_tabla_comentarios_1.png)

Creamos las llaves foráneas para los comentarios de los usuarios

![platziblog_tabla_comentarios_usuarios_fk_1.png](src/platziblog_tabla_comentarios_usuarios_fk_1.png)

![platziblog_tabla_comentarios_usuarios_fk_2.png](src/platziblog_tabla_comentarios_usuarios_fk_2.png)

Creamos las llaves foráneas para los comentarios de los posts

![platziblog_tabla_comentarios_usuarios_fk_1.png](src/platziblog_tabla_comentarios_usuarios_fk_1.png)

![platziblog_tabla_comentarios_usuarios_fk_2.png](src/platziblog_tabla_comentarios_usuarios_fk_2.png)

Ahora solo nos queda crear la tabla intermedia para romper la relacion muchos a muchos.

![diagrama_fisico_paso_3_N_N.png](src/diagrama_fisico_paso_3_N_N.png)

Para ello creamos la tabla intermedia post_etiquetas

![platziblog_tabla_post_etiquetas.png](src/platziblog_tabla_post_etiquetas.png)

![platziblog_tabla_post_etiquetas_1.png](src/platziblog_tabla_post_etiquetas_1.png)

Ligamos las llaves foráneas para post_id

![platziblog_tabla_post_etiquetas_fk_1.png](src/platziblog_tabla_post_etiquetas_fk_1.png)

![platziblog_tabla_post_etiquetas_fk_2.png](src/platziblog_tabla_post_etiquetas_fk_2.png)

Ligamos las llaves foráneas para etiquetas_id

![platziblog_tabla_post_etiquetas_etiquetas_fk_1.png](src/platziblog_tabla_post_etiquetas_etiquetas_fk_1.png)

![platziblog_tabla_post_etiquetas_etiquetas_fk_2.png](src/platziblog_tabla_post_etiquetas_etiquetas_fk_2.png)

#### Reverse Engineer

Seleccionamos la opción Database para acceder a reverse engineer
![reverse_engineer_1](src/reverse_engineer_1.png)

![reverse_engineer_2](src/reverse_engineer_2.png)

![reverse_engineer_3](src/reverse_engineer_3.png)

![reverse_engineer_4](src/reverse_engineer_4.png)

![reverse_engineer_5](src/reverse_engineer_5.png)

![reverse_engineer_6](src/reverse_engineer_6.png)

![reverse_engineer_7](src/reverse_engineer_7.png)

### Clase 28 Por qué las consultas son tan importantes

Las consultas o queries a una base de datos son una parte fundamental ya que esto podría salvar un negocio o empresa.
Alrededor de las consultas a las bases de datos se han creado varias especialidades como ETL o transformación de datos, business intelligence e incluso machine learning.

### Clase 29 Estructura básica de un Query

Los queries son la forma en la que estructuramos las preguntas que se harán a la base de datos. Transforma preguntas en sintaxis.

El query tiene básicamente 2 partes: SELECT y FROM y puede aparecer una tercera como WHERE.

La estrellita o asterisco (*) quiere decir que vamos a seleccionar todo sin filtrar campos.

Antes de iniciar la clase corre este script

```sql
Script de la base datos platziblog

--creamos la base datos :platziblog

-- nos ubicamos en la base datos  platziblog
use platziblog;

-- CREACIONES DE TABLAS
-- Eliminacion de tablas, va en ese orden por los FK
 drop table comentarios;
 drop table posts_etiquetas;
 drop table posts;
 drop table etiquetas;
 drop table usuarios;
 drop table categorias;


-- CREACIONES DE TABLAS
-- Creación de la tabla usuarios
CREATE TABLE `usuarios` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `login` varchar(30) NOT NULL,
  `password` varchar(32) NOT NULL,
  `nickname` varchar(40) NOT NULL,
  `email` varchar(40) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY`email_UNIQUE` (`email`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- Creación de la tabla categorias
CREATE TABLE `categorias` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `nombre_categoria`varchar(30) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- Creación de la tabla etiquetas
CREATE TABLE`etiquetas` (
  `id`int(11) NOT NULL AUTO_INCREMENT,
  `nombre_etiqueta`varchar(30) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- Creación de la tabla posts
CREATE TABLE `posts` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `titulo` varchar(130) NOT NULL,
  `fecha_publicacion` timestamp NULL DEFAULT NULL,
  `contenido` text NOT NULL,
  `estatus` char(8) DEFAULT 'activo',
  `usuario_id` int(11) DEFAULT NULL,
  `categoria_id` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`),
  KEY `posts_usuarios_idx` (`usuario_id`),
  KEY `posts_categorias_idx` (`categoria_id`),
  CONSTRAINT `posts_categorias` FOREIGN KEY (`categoria_id`) REFERENCES `categorias` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION,
  CONSTRAINT `posts_usuarios` FOREIGN KEY (`usuario_id`) REFERENCES `usuarios` (`id`) ON DELETE NO ACTION ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;

-- Creación de la tabla comentarios
CREATE TABLE `comentarios` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `cuerpo_comentario` text NOT NULL,
  `usuario_id` int(11) NOT NULL,
  `post_id` int(11) NOT NULL,
  PRIMARY KEY (`id`),
  KEY `comentarios_usuario_idx` (`usuario_id`),
  KEY `comentarios_post_idx` (`post_id`),
  CONSTRAINT `comentarios_post` FOREIGN KEY (`post_id`) REFERENCES `posts` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION,
  CONSTRAINT `comentarios_usuario` FOREIGN KEY (`usuario_id`) REFERENCES `usuarios` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION
) ENGINE=InnoDB DEFAULT CHARSET=utf8;


-- Creación de la tabla posts_etiquetas
CREATE TABLE `posts_etiquetas` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `post_id` int(11) NOT NULL,
  `etiqueta_id` int(11) NOT NULL,
  PRIMARY KEY (`id`),
  KEY `postsetiquetas_post_idx` (`post_id`),
  KEY `postsetiquetas_etiquetas_idx` (`etiqueta_id`),
  CONSTRAINT `postsetiquetas_etiquetas` FOREIGN KEY (`etiqueta_id`) REFERENCES `etiquetas` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION,
  CONSTRAINT `postsetiquetas_post` FOREIGN KEY (`post_id`) REFERENCES `posts` (`id`) ON DELETE NO ACTION ON UPDATE NO ACTION
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=utf8;


-- INSERCIÓN DE VALORES A LAS TABLAS
-- Insert  en la tabla usuarios
INSERT INTO usuarios (login,password,nickname,email) VALUES ('israel','1234','israel','israel@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('monica','1234','Moni','monica@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('laura','1234','Lau','laura@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('edgar','5678','Ed','edgar@platziblog.com');
INSERT INTO usuarios (login,password,nickname,email) VALUES ('perezoso','5678','Oso Pérez','perezoso@platziblog.com');

-- Insert  en la tabla categorias
INSERT INTO categorias (nombre_categoria) VALUES ('Ciencia');
INSERT INTO categorias (nombre_categoria) VALUES ('Tecnología');
INSERT INTO categorias (nombre_categoria) VALUES ('Deportes');
INSERT INTO categorias (nombre_categoria) VALUES ('Espectáculos');
INSERT INTO categorias (nombre_categoria) VALUES ('Economía');

-- Insert  en la tabla etiquetas
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Robótica');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Computación');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Teléfonos Móviles');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Automovilismo');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Campeonatos');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Equipos');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Bolsa de valores');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Inversiones');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Brokers');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Celebridades');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Eventos');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Moda');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Avances');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Nobel');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Matemáticas');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Química');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Física');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Largo plazo');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Bienes Raíces');
INSERT INTO etiquetas (nombre_etiqueta) VALUES ('Estilo');

