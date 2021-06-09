---
title: Fundamentos de la Programación
theme: sky
slideNumber: true
---

# Bibliotecas o Librerias

Created by <i class="fab fa-telegram"></i>
[edme88](https://t.me/edme88)

---
### Bibliotecas
Las bibliotecas contienen el código objeto de muchos programas que permiten hacer cosas comunes, como leer el teclado, 
escribir en la pantalla, manejar números, realizar funciones matemáticas, etc.

Permiten reutilizar funciones presumiblemente comprobadas, ahorrando tiempo de desarrollo e incrementando la fiabilidad del programa.

---
### Bibliotecas
Las bibliotecas están clasificadas por el tipo de trabajos que hacen, hay bibliotecas de entrada y salida, matemáticas, 
de manejo de memoria, de manejo de textos y como imaginarás existen muchísimas librerías disponibles y todas con una 
función especifica.

---
### Bibliotecas
Las librerías no son únicamente archivos externos creados por otros, también es posible crear nuestras propias librerías 
y utilizarlas en nuestros programas. Las librerías pueden tener varias extensiones diferentes, las más comunes son: 
.lib, .bpl, .a, .dll, .h y algunas más ya no tan comunes.

---
### Bibliotecas
La declaración de librerías, se debe hacer al principio de todo nuestro código, antes de la declaración de cualquier función o línea de código, debemos indicarle al compilador que librerías usar, para el saber que términos estaran correctos en la escritura de nuestro código y cuáles no. La sintaxis es la siguiente: #include <nombre de la librería> 

---
### Bibliotecas: Ejemplos
Algunos ejemplos de bibliotecas son:
* <a href="#/6">iostream</a>
* <a href="#/8">cstdio</a>
* <a href="#/9">cmath</a>
* <a href="#/14">cstdlib</a>
* <a href="#/16">cctype</a>
* <a href="#/19">ctime</a>
* <a href="#/20">string</a>

---
### [iostream](http://www.cplusplus.com/reference/iolibrary/)
Se emplea para operaciones de entrada/salida. Su nombre es el acrónimo de **I**nput/**O**utput **Stream**.
El flujo de entrada y salida de datos no se encuentra definida dentro de la sintaxis básica y se provee por
medio de librerías de funciones especializadas como iostream.

---
### iostream
* cin: Flujo de entrada
* cout: Flujo de salida
* cerr: Flujo de error no almacenado
* clog: Flujo de error almacenado
Todos los objetos derivados de iostream hacen parte del espacio de nombres std.

---
### [cstdio](http://www.cplusplus.com/reference/cstdio/?kw=cstdio)
Biblioteca "Standard Input Output Header" de entrada/salida, que incluye funciones necesarias para escribir y leer. (se usa en C)
* printf: imprimir salidas de datos
* scanf: utilizado para introducir datos de entrada
* puts: imprime una cadena de caracteres
* getc: devuelve un caracter desde un fichero
* ferror: comprueba el indicador de errores

---
### [cmath](http://www.cplusplus.com/reference/cmath/?kw=cmath)
Biblioteca estándar con operaciones matemáticas básicas: arcocoseno, arcoseno, arcotangente, coseno,
coseno hiperbólico, exponencial, valor absoluto, logaritmo natural y base 10, seno, seno hiperbólico, raíz cuadrada, tangente, tangente hiperbólica.

---
### cmath
| Nombre | Descripción |
|--------|-------------|
| acos | Calcula el arcocoseno. |
| asin | Calcula el arcoseno. |
| atan | Calcula la arcotangente. |
| atan2 | Calcula la arcotangente de dos parámetros. |
| floor | Devuelve el menor entero no menor que el parámetro. |

---
### cmath
| Nombre | Descripción |
|--------|-------------|
| ceil | Devuelve el mayor entero no mayor que el parámetro. |
| cos | Calcula el coseno. |
| cosh | Calcula el coseno hiperbólico. |
| exp(double x) | Devuelve el valor del número e elevado a la potencia x. |
| fabs | Devuelve el valor absoluto. |

---
### cmath
| Nombre | Descripción |
|--------|-------------|
| fmod | Devuelve el resto de la división de flotantes |
| frexp | Realiza la fracció y eleva al cuadrado. |
| labs | Calcula el valor absoluto. |
| ldexp | Devuelve tamaño del exponente de un valor en punto flotante. |
| log | Calcula el logaritmo natural. |
| log10 | Calcula el logaritmo en base 10 |

---
### cmath
<!-- .slide: style="font-size: 0.9em" -->
| Nombre | Descripción |
|--------|-------------|
| modf | Devuelve un valor en punto flotante íntegro y en partes. |
| pow(x,y) | Eleva un valor dado a un exponente, xy |
| sin | Calcula el seno |
| sinh | Calcula el seno hiperbólico |
| sqrt | Calcula la raíz cuadrada |
| tan | Calcula la tangente |
| tanh | Calcula la tangente hiperbólica |

---
### [cstdlib](http://www.cplusplus.com/reference/cstdlib/?kw=cstdlib)
<!-- .slide: style="font-size: 0.9em" -->
Standard library. Contiene los prototipos de funciones de C para gestión de memoria dinámica, control de procesos y otras.

Contiene funciones para:
* Conversión de caracteres a: float, int, long, double
* Números Aleatorios
* Memoria 
* Control de procesos
* Ordenación 
* Búsqueda

---
### cstdlib
* atof: ascii to float, cadena de caracteres a coma flotante
* rand: genera un numero pseudo-aleatorio
* free: liberan memoria devolviéndola al heap
* system: ejecutar un comando externo
* exit: terminar ejecución del programa

---
### [cctype](http://www.cplusplus.com/reference/cctype/?kw=cctype)
<!-- .slide: style="font-size: 0.9em" -->
Contiene funciones de manipulación de caracteres:

| Funcion | Detalle |
|---------|---------|
| isalnum | Verifica si el caracter es alphanumeric |
| isalpha | Verifica si el caracter es alphabetic |
| isblank | Verifica si el caracter es blank |
| iscntrl | Verifica si el caracter es a control character |
| isdigit | Verifica si el caracter es decimal digit |

---
### cctype
<!-- .slide: style="font-size: 0.9em" -->
| Funcion | Detalle |
|---------|---------|
| isdigit | Verifica si el caracter es decimal digit |
| isgraph | Check if character has graphical representation |
| islower | Verifica si el caracter es lowercase letter |
| isprint | Verifica si el caracter es printable |
| ispunct | Verifica si el caracter es a punctuation character |

---
### cctype
<!-- .slide: style="font-size: 0.9em" -->
| Funcion | Detalle |
|---------|---------|
| isspace | Verifica si el caracter es a white-space |
| isupper | Verifica si el caracter es uppercase letter |
| isxdigit | Verifica si el caracter es hexadecimal digit |
| tolower | Convierte uppercase letter a lowercase |
| toupper | Convierte lowercase letter a uppercase |
| toascii | Convierte de char a Ascii |

---
### [ctime](http://programavideojuegos.blogspot.com/2014/02/la-libreria-timeh.html)
Contiene funciones para manipular fecha y hora del sistema.

<!-- .slide: style="font-size: 0.8em" -->
| Funcion | Detalle |
|---------|---------|
| clock_t clock (void) | Devuelve el número de pulsos de reloj desde que se inició el proceso |
| double difftime(time_t, time t) | Recibe dos variables de tipo time_t, calcula su diferencia y devuelve el resultado (double) expresado en segundos. |
| etc | etc |

---
### [string](http://www.cplusplus.com/reference/string/string/?kw=string)
Contiene la definición de macros, constantes, funciones y tipos y algunas operaciones de manipulación de memoria.

Las funciones para cadenas de caracteres sólo trabajan con conjuntos de caracteres ASCII o extensiones ASCII compatibles.

* strcpy: copia una cadena en otra
* strcat: añade una cadena al final de otra.
* strrev: invierte una cadena
* strstr: busca una cadena dentro de otra.

---
### Generar Numeros Aleatorios
````javascript
#include <stdlib.h>
#include <time.h>
#include<iostream>
using namespace std;
 
int main()
{
    int num, c;
    srand(time(NULL)); //inicializar los números aleatorios
    
    for(c = 1; c <= 10; c++)
    {
        num = 1 + rand() % (11 - 1); //Números Aleatorios entre 1 a 10
        cout<<num<< " ";
    }
    
    //num=rand()%51; Número Aleatorio entre 0 a 50
    //De forma General es:
    //variable = limite_inferior + rand() % (limite_superior +1 - limite_inferior) ;
}
````

---
## ¿Dudas, Preguntas, Comentarios?
![DUDAS](images/pregunta.gif)
