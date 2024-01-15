---
title: juanj-mata-go
created: '2024-01-14T15:21:23.680Z'
modified: '2024-01-15T04:55:23.737Z'
---

<div style="page-break-after: always;"></div>

# GO

[//]: # (version: 1.0)
[//]: # (author: Juan José Mata)
[//]: # (date: 2024-01-14)

---
# Indice
- [GO](#go)
- [Indice](#indice)
- [Enlaces de interes](#enlaces-de-interes)
- [Introducción](#introducción)
  - [Historia de GO](#historia-de-go)
    - [Que es GO y sus caracteristicas](#que-es-go-y-sus-caracteristicas)
- [Instalación](#instalación)
  - [Instalación de GO](#instalación-de-go)
    - [Instalación en Windows](#instalación-en-windows)
    - [Instalación en Linux](#instalación-en-linux)
    - [Instalación en MacOS](#instalación-en-macos)
  - [Instalación del IDE Visual Studio Code](#instalación-del-ide-visual-studio-code)
    - [Instalación en Windows](#instalación-en-windows-1)
    - [Instalación en Linux](#instalación-en-linux-1)
    - [Instalación en MacOS](#instalación-en-macos-1)
    - [Extensiones recomendadas](#extensiones-recomendadas)
- [Hola Mundo](#hola-mundo)
- [Conceptos basicos](#conceptos-basicos)
  - [Paquetes e importaciones](#paquetes-e-importaciones)
  - [Convención de nomenclaturas](#convención-de-nomenclaturas)
  - [Comentarios](#comentarios)
  - [Tipos de datos](#tipos-de-datos)
    - [Enteros](#enteros)
    - [Flotantes](#flotantes)
    - [Booleanos](#booleanos)
    - [Strings](#strings)
  - [Operadores](#operadores)
    - [Operadores aritméticos](#operadores-aritméticos)
    - [Operadores logísticos](#operadores-logísticos)
    - [Operadores de comparación](#operadores-de-comparación)
- [Variables](#variables)
  - [Inicializar y reasignación](#inicializar-y-reasignación)
  - [Variables según su ambito](#variables-según-su-ambito)
    - [Variables locales](#variables-locales)
    - [Variables globales](#variables-globales)
- [Constantes](#constantes)
- [Arrays](#arrays)
- [Estructuras de control](#estructuras-de-control)
  - [Condicionales](#condicionales)
    - [If, else y else if](#if-else-y-else-if)
    - [Switch](#switch)
  - [Bucles](#bucles)
    - [While y do while](#while-y-do-while)
    - [For](#for)
  - [GOTO](#goto)
- [Funciones](#funciones)
- [Structs](#structs)
- [Programación orientada a objetos (POO)](#programación-orientada-a-objetos-poo)
- [CRUD](#crud)
  - [Capitulo 2](#capitulo-2)
    - [Subapartado 2.1](#subapartado-21)
  - [Capitulo 3](#capitulo-3)
    - [Seccion1](#seccion1)
    - [Seccion2](#seccion2)
      - [Seccion2.1](#seccion21)

---
# Enlaces de interes
[Volver al indice](#indice)

- [Web oficial](https://go.dev/)
- [Zona de descargas](https://go.dev/dl/)
- [Documentación oficial](https://go.dev/doc/)
- [Wikipedia](https://es.wikipedia.org/wiki/Go_(lenguaje_de_programaci%C3%B3n))
- [Librerias estandar](https://pkg.go.dev/std)
- [Ejemplos](https://gobyexample.com/)

---
# Introducción
[Volver al indice](#indice)

## Historia de GO

La compañía Google, conocida por dar múltiples servicios en internet, como puede ser su famoso buscador [www.google.es](www.google.es), es una empresa que maneja una gran variedad de proyectos.

Antes de que existiera Go, Google usaba para sus proyectos sobre todo lenguajes de bajo nivel como podían ser C o C++. En el año 2007 tres de sus desarrolladores (Rob Pike, Robert Griesemer y Ken Thompson) se pusieron manos a la obra y cogieron lo mejor del lenguaje C y lo mejor del lenguaje Python para sentar las bases para un nuevo lenguaje de programación. Dos años después, en el 2009, Google lanzo oficialmente el lenguaje de programación bautizado como Go, aunque también es conocido como Golang o Google Go.

Go nació con el objetivo de aprender y no cometer los mismos errores que cometían otros lenguajes de programación mas antiguos, por ellos se cogió lo mejor de cada uno y se eliminaros problemas y limitaciones que estos presentaban.

En la actualidad Go es usado por multitud de compañías como por ejemplo Paypal, Dropbox, Netflix, Uber, Twitch, etc, y lógicamente por su creadora, Google.

### Que es GO y sus caracteristicas

Go es un lenguaje de programación desarrollado por Google que nacio con el principal objetivo de ser un lenguaje bastante simple, pero al mismo tiempo ser muy eficiente. Este año 2024 cumple 15 años, lo que significa que en comparación con otros lenguaje de programación como C o Java, se trata de un lenguaje joven.

Caracteristicas:

- Simplicidad: Tiene una sintaxis clara y organizada.
- Muy facil de usar
- OpenSource: Es un lenguaje de codigo abierto.
- Lenguaje compilado: El codigo fuente se compila generando codigo maquina y así ejecutar el programma.
- Usa tipado estatico: Una vez se le asigna un tipo de dato a una variable esta ya no puede cambiar.
- No esta orientado a objetos (POO), pero tiene formas de emularlo
- Es multiprocesador y concurrente: Permite ejecutar multiples procesos paralelamente en cada uno de los procesadores del equipo.

---
# Instalación
[Volver al indice](#indice)

## Instalación de GO

Go se puede instalar en cualquier sistema operativo. Accede a [la zona de descargas](https://go.dev/dl/) de la web oficial de GO.

Una vez en la zona de descargas tienes disponible la sección “Featured downloads” en la cual aparecen los paquetes de instalación de los sistemas operativos con sus arquitecturas más comunes.

También está la sección “Stable versions” donde se encuentra un listado completo de paquetes de instalación en sus últimas versiones estables organizados por sistema operativo y por arquitecturas.

Si en la sección “featured downloads” no aparece el paquete que coincida con tu sistema operativo y arquitectura, en la sección “Stable versions” lo encontraras.

Por último, está la sección “Unstable versión” donde puedes descargar los paquetes de instalación de versiones no estables (No recomendado).

En el momento de hacer esta documentación (enero del 2024) la versión estable mas actualizada es la 1.21.6.

### Instalación en Windows

En Windows la forma de instalar GO es muy simple. En la zona de descargas de la pagina web oficial de GO debes  [descargar el paquete de Windows](https://go.dev/dl/go1.21.6.windows-amd64.msi) y ejecutarlo para iniciar la instalación.

El proceso de instalación se resume en pulsar “siguiente” en las pantallas por lo que no tiene ninguna dificultad.

Una vez finalizada la instalación puedes confirmar que esta se ha realizado correctamente abriendo una consola CMD y ejecutando el comando:

```console
go versión
```

Debería aparecer un mensaje indicándote la versión instalada, que en este caso debería ser la 1.21.6.

### Instalación en Linux

Para instalar Go en linux abre una consola de comandos y ejecuta los siguientes comandos:

```console
# Te situas en la carpeta de descargas
cd Descargas
# Descargas el paquete de instalación
wget https://go.dev/dl/go1.21.6.linux-amd64.tar.gz
# Copias el paquete en la ruta /usr/local
sudo cp go1.21.6.linux.amd64.tar.gz /usr/local
# Te situas en la carpeta /usr/local
cd ~
cd /usr/local
# Creas la carpeta GO y descomprimes en ella el paquete
sudo rm -rf /usr/local/go && sudo tar -C /usr/local -xzf go1.21.6.linux-amd64.tar.gz
```

El siguiente paso es añadir acceso de variable de global:

```console
export PATH=$PATH:/usr/local/go/bin
```

Para confirmar que se ha añadido correctamente ejecutamos el siguiente comando:

```console
echo $PATH
```

Si aparece “/usr/local/go/bin” significa que funcionó correctamente.

Finalmente, para confirmar que GO esta instalado, ejecuta el comando:

```console
go versión
```

Debería aparecer un mensaje indicando la versión instalada, que en este caso debería ser la 1.21.6.


### Instalación en MacOS

Para instalar GO en un equipo con MacOS puedes usar el mismo método que con el sistema operativo Windows.

En la zona de descargas de la página web oficial de GO descargas el [paquete de instalación de MacOS para ARM64](https://go.dev/dl/go1.21.6.darwin-arm64.pkg) o [el paquete de instalación de MacOS para x86-64](https://go.dev/dl/go1.21.6.darwin-amd64.pkg) y lo ejecutas para iniciar la instalación.

El proceso de instalación se resume en pulsar “siguiente” en las pantallas por lo que no tiene ninguna dificultad.

Una vez finalizada la instalación puedes confirmar que esta se ha realizado correctamente abriendo una consola CMD y ejecutando el comando:

```console
go versión
```

Debería aparecer un mensaje indicándote la versión instalada, que en este caso debería ser la 1.21.6.


## Instalación del IDE Visual Studio Code

Para empezar a programar con GO primero debemos decidir que Entorno de desarrollo (IDE) vamos a usar.

Existe un IDE llamado [GoLand](https://www.jetbrains.com/go/) el cual fue creado en exclusiva para ser usado junto con Go, pero por desgracia se trata de un IDE de pago.

Existen muchas opciones, pero el IDE mas usado en la actualidad y que además es compatible con GO es Visual Studio Code, por lo que es el que recomiendo.


### Instalación en Windows

Para instalar Visual Studio Code debes acceder a la [zona de descargas](https://code.visualstudio.com/Download) de su pagina web oficial , pulsar en el botón donde pone “Windows” y [descargar el paquete de instalación](https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-user).

En el momento de realizar esta documentación la versión mas actualizada es la 1.85.

Una vez descargado debes ejecutar el paquete de instalación. El proceso de instalación se resume en pulsar “siguiente” en las pantallas por lo que no tiene ninguna dificultad. 

### Instalación en Linux

Para realizar la instación de Visual Studio Code en linux abre una consola y ejecuta los siguientes comandos:

```console
sudo apt update
sudo apt install software-properties-common apt-transport-https wget
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install code
```

### Instalación en MacOS

Para instalar Visual Studio Code debes acceder a la [zona de descargas](https://code.visualstudio.com/Download) de su página web oficial, pulsar en el botón donde pone “Mac” y [descargar el paquete de instalación](https://code.visualstudio.com/sha/download?build=stable&os=darwin-universal).

En el momento de realizar esta documentación la versión mas actualizada es la 1.85.

Una vez descargado debes ejecutar el paquete de instalación. El proceso de instalación se resume en pulsar “siguiente” en las pantallas por lo que no tiene ninguna dificultad.


### Extensiones recomendadas

Una vez tengas instalado el IDE Visual Studio Code, lo primero que harás es ir a la sección de extensiones (Control + Mayus + X), escribir “go” e instalar la primera extensión que aparece.

La extensión “GO” añadirá funciones extras a Visual Studio Code cuando estes programando con el lenguaje GO, como por ejemplo IntelliSense.

Si tras la instalación de la extensión "go” o cuando empieces a generar tus primeros códigos de GO aparece en la esquina de abajo a la derecha algún mensaje indicándote que hace falta instalar alguna extensión extra, no lo dudes y pulsa el botón instalar ya que te hará falta.

También sería recomendable que instalaras la extensión “Spanish Languaje Pack for Visual Studio Code” para que tengas el IDE en español.


---
# Hola Mundo
[Volver al indice](#indice)

Como suele ser común con todos los lenguajes de programación, el primer código que probaras será el famoso “Hola Mundo”.

Para ello lo primero será crear una carpeta en el directorio que tú quieras de tu ordenador, teniendo en cuenta que esa carpeta será donde vas a guardar tus proyectos en GO.

Una vez creada la carpeta, en Visual Studio Code debes ir a “Archivo > Agregar carpeta al área de trabajo” y seleccionar la carpeta que acabas de crear.

Lo siguiente será crear un archivo dentro de la carpeta, al que llamaremos “HolaMundo.go”.

Para generar el primer Hola Mundo debes escribir el siguiente código:

```GO
package main

import "fmt"

func main() {
    fmt.Println("Hola mundo")
}
```

Para ejecutarlo debes pulsar el botón “Run code” que se encuentra en la parte superior derecha de Visual Studio Code, o usar el atajo de teclado Control + Alt + N.

El resultado será que se muestre por consola el mensaje “Hola mundo”.

# Conceptos basicos
## Paquetes e importaciones
## Convención de nomenclaturas
## Comentarios
## Tipos de datos
### Enteros
### Flotantes
### Booleanos
### Strings
## Operadores
### Operadores aritméticos
### Operadores logísticos
### Operadores de comparación

---
# Variables
[Volver al indice](#indice)

## Inicializar y reasignación
## Variables según su ambito
### Variables locales
### Variables globales

---
# Constantes
[Volver al indice](#indice)

---
# Arrays
[Volver al indice](#indice)

---
# Estructuras de control
[Volver al indice](#indice)

## Condicionales
### If, else y else if
### Switch

## Bucles
### While y do while
### For

## GOTO

---
# Funciones
[Volver al indice](#indice)

---
# Structs
[Volver al indice](#indice)

---
# Programación orientada a objetos (POO)
[Volver al indice](#indice)

---
# CRUD
[Volver al indice](#indice)

---
---
---




## Capitulo 2
[Tabla de contenidos](#tabla-de-contenidos)

### Subapartado 2.1
[Tabla de contenidos](#tabla-de-contenidos)

<div style="page-break-after: always;"></div>


## Capitulo 3
[Tabla de contenidos](#tabla-de-contenidos)

- Recursos: 
  - 

```php
echo "Hola Mundo";
```

### Seccion1
[Tabla de contenidos](#tabla-de-contenidos)

```console

```



### Seccion2
[Tabla de contenidos](#tabla-de-contenidos)

```console
#...
```


#### Seccion2.1
[Tabla de contenidos](#tabla-de-contenidos)

1. **negrita**

```console
sudo apt update
sudo apt upgrade
```


<a id="s22">Seccion2.2</a>

[Tabla de contenidos](#indice)

1. **negrita**

```console
sudo apt update
sudo apt upgrade
```
