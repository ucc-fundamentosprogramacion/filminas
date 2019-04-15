---
title: Fundamentos de la Programación
theme: black
slideNumber: true
---

# Bibliotecas
<small>
Created by <i class="fab fa-telegram"></i>
[edme88]("https://t.me/edme88") & 
<i class="fab fa-telegram"></i>
[rmarku]("https://t.me/rmarku")
</small>

---
### Bibliotecas
Permiten reutilizar funciones presumiblemente comprobadas, ahorrando tiempo de desarrollo e incrementando la fiabilidad del programa.

---
### Bibliotecas: Ejemplos
Algunos ejemplos de bibliotecas son:
* stdio.h
* math.h
* iostream
* stdlib.h o cstdlib
* ctype.h
* time.h

---
### stdio.h
Biblioteca "Standard Input Output Header" de entrada/salida, que incluye funciones printf y scanf necesarias para escribir y leer. (se usa en C)

---
### math.h
Biblioteca estándar con operaciones matemáticas básicas: arcocoseno, arcoseno, arcotangente, coseno,
coseno hiperbólico, exponencial, valor absoluto, logaritmo natural y base 10, seno, seno hiperbólico, raíz cuadrada, tangente, tangente hiperbólica.

---
### math.h
| Nombre | Descripción |
|--------|-------------|
| acos | Calcula el arcocoseno. |
| asin | Calcula el arcoseno. |
| atan | Calcula la arcotangente. |
| atan2 | Calcula la arcotangente de dos parámetros. |
| floor | Devuelve el menor entero no menor que el parámetro. |
| ceil | Devuelve el mayor entero no mayor que el parámetro. |
| cos | Calcula el coseno. |
| cosh | Calcula el coseno hiperbólico. |
| exp(double x) | Devuelve el valor del número e elevado a la potencia x. |
| fabs | Devuelve el valor absoluto. |
| fmod | Devuelve el resto de la división de flotantes |
| frexp | Realiza la fracció y eleva al cuadrado. |
| labs | Calcula el valor absoluto. |
| ldexp | Devuelve tamaño del exponente de un valor en punto flotante. |
| log | Calcula el logaritmo natural. |
| log10 | Calcula el logaritmo en base 10 |
| modf | Devuelve un valor en punto flotante íntegro y en partes. |
| pow(x,y) | Eleva un valor dado a un exponente, xy |
| sin | Calcula el seno |
| sinh | Calcula el seno hiperbólico |
| sqrt | Calcula la raíz cuadrada |
| tan | Calcula la tangente |
| tanh | Calcula la tangente hiperbólica |

---
### stdlib.h o cstdlib
Contiene funciones para:
* Conversión de caracteres a: float, int, long, double
* Números Aleatorios
* Memoria 
* Control de procesos
* Ordenación 
* Búsqueda 
* Matemáticas: división 

---
### ctype.h
Contiene funciones de manipulación de caracteres:
| Funcion | Detalle |
|---------|---------|
| isalnum | Verifica si el caracter es alphanumeric |
| isalpha | Verifica si el caracter es alphabetic |
| isblank | Verifica si el caracter es blank |
| iscntrl | Verifica si el caracter es a control character |
| isdigit | Verifica si el caracter es decimal digit |
| isgraph | Check if character has graphical representation |
| islower | Verifica si el caracter es lowercase letter |
| isprint | Verifica si el caracter es printable |
| ispunct | Verifica si el caracter es a punctuation character |
| isspace | Verifica si el caracter es a white-space |
| isupper | Verifica si el caracter es uppercase letter |
| isxdigit | Verifica si el caracter es hexadecimal digit |
| tolower | Convierte uppercase letter a lowercase |
| toupper | Convierte lowercase letter a uppercase |
| toascii | Convierte de char a Ascii |

---
### [time.h}(http://programavideojuegos.blogspot.com/2014/02/la-libreria-timeh.html)
Contiene funciones para manipular fecha y hora del sistema.

| Funcion | Detalle |
|---------|---------|
| clock_t clock (void) | Devuelve el número de pulsos de reloj desde que se inició el proceso |
| double difftime(time_t, time t) | Recibe dos variables de tipo time_t, calcula su diferencia y devuelve el resultado (double) expresado en segundos. |
| etc | etc |

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
