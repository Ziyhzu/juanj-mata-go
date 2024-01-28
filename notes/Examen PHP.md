---
title: Examen PHP
created: '2024-01-23T16:39:43.099Z'
modified: '2024-01-23T17:08:17.856Z'
---

# Examen PHP
- Alumno: Juan José Mata

[//]: # (version: 1.0)
[//]: # (author: Juan José Mata)
[//]: # (date: 2024-01-23)

---
##  Lógica de la base de datos

- Hay **5 entidades**, de las cuales 3 son fuertes (Clientes, Empleados y Vehículos) y 2 son débiles (Repuestos y Ventas).

- Ventas recibe llaves foráneas de Clientes, Empresas y Vehículos, mientras que Repuestos recibe su clave foránea de Vehículos.

- Las 5 entidades tienen un campo llamado **“activo”** que sirve para realizar los borrados lógicos.

- En el momento de crear las tablas de las entidades se da a las claves foráneas los valores **ON UPDATE CASCADE y ON DELETE SET NULL** para controlar los datos en caso de ser editados o eliminados.


## Lógica del proyecto

- La estructura del proyecto gira en torno a 2 conceptos: **Modularización y que todo se gestione desde el index.php**.

- En lugar de generar un archivo PHP lleno de código se ha optado por generar más archivos pero que cada uno cumpla una función determinada. La idea es que si en un futuro hubiera que modificar algo se podría hacer sin riesgo a afectar al resto del proyecto.

- Gracias a la modularización y a **“include”** conseguimos que sin movernos de index.php se ejecute y se pinte por pantalla todo lo que se necesita.

## Estructura

- En la raíz de la carpeta del proyecto está index.php, el archivo .sql con la base de datos y un conjunto de archivos select, insert, update, delete fisico, delete logico y off (para visualizar registros borrados) por cada entidad de la base de datos.

- También está la carpeta img, donde se guardan las imágenes necesarias para el frontend, y la carpeta php donde se almacenan archivos que dan funcionalidad al proyecto.


## Funcionamiento

- Dentro de index.php hay un primer fragmento de código que le aporta estética a la portada [basada en hyundauto](https://www.hyundai.es/concesionarios/hyundauto) y que **siempre estará presente**.

- A continuación hay un condicional IF que en caso de no tener una sesión iniciada cargara en pantalla los módulos de carga de base de datos y login. Una vez se inicia sesión, se activa el condicional ELSE el cual carga el módulo de menú que se usara para acceder al CRUD y sus distintas opciones. Junto al menú hay un botón que permite el cierre de sesión y volver al condicional de no haber una sesión iniciada y mostrar el login.

- Si se hace click en alguna de las opciones del menú se carga en la URL **“?url=x”** (siendo x la entidad de la cual queremos cargar el CRUD). Haciendo uso de **$_GET[“url”]** se consigue capturar lo que ha seleccionado el usuario y cargar con include el modulo PHP que sea oportuno.

- El CRUD de cada entidad muestra los datos activos, permitiendo insertar, modificar, eliminar de manera lógica y eliminar de manera física los registros. También se puede acceder a los registros desactivados y volver a activarlos.

