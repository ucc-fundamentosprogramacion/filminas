---
title: Fundamentos de la Programación
theme: sky
slideNumber: true
---

# Comenzar en C++

Created by <i class="fab fa-telegram"></i>
[edme88](https://t.me/edme88)

---
## Entorno de Desarrollo
Es una herramienta que nos permite desarrollar nuestro programa.

Cuenta con un editor de texto y compilador.

---
## Entorno de Desarrollo
* Code::Blocks
* C-Lion
* Zinjal
* Visual Studio
* Code Board
* NetBeans
* Eclipse
etc, etc...

---
## Code Blocks
Descargar el Code::Blocks del siguiente link: [http://www.codeblocks.org/downloads/26](http://www.codeblocks.org/downloads/26)
![Code::Blocks](images/U3_programacion/Descargar_code.png)
Asegurate de que sea la versión que incluye el **mingw** que incluye el compilador.

---
### Code Blocks: Compilador
El compilador traducirá el código fuente a código máquina, también llamado código objeto, siempre y cuando, 
el propio compilador no detecte ningún error en dicho código fuente.
![Code::Blocks](images/U3_programacion/config_compilador.png)

---
### Code Blocks: Compilador
![Code::Blocks](images/U3_programacion/config_compilador2.png)

---
## Alternativa: Codeboard.io
Puedes crearte una cuenta de [https://codeboard.io](https://codeboard.io)
![Code Board](images/U3_programacion/codeboard.png)

---
## Code Blocks
![Code Blocks](images/U3_programacion/code_blocks_1.png)

---
## Comenzando
````javascript
/*
Fundamentos de Programacion
Autor: Nombre Apellido
Consigna
*/
#include <iostream>
using namespace std;

int main(){
    cout << "Hola mundo" << endl;
    return 0;
}
````

---
## Include
Instrucción al preprocesador que se usa para adicionar un archivo al código, como por ejemplo la llamada a una biblioteca 
de funciones en C++.

````javascript
#include <iostream>
````
Antes del proceso de compilación, el preprocesador es llamado primero a ejecutarse y buscar llamadas de instrucción 
al pre-procesador.

---
## Include
La instrucción **include** le indica al preprocesador que cuando este se ejecute, el compilador debe incluir un archivo en el código.

Este archivo suele ser: bibliotecas, secuencias, funciones y objetos, etc.

---
## Using namespace std
Al incluir la sentencia  
````javascript
using namespace std;
````
le estamos diciendo al compilador que usaremos el espacio de nombres std por lo que no tendremos que incluirlo 
cuando usemos elementos de este espacio de nombres, como pueden ser los objetos **cout** y **cin**, que representan el 
flujo de salida estándar (típicamente la pantalla o una ventana de texto) y el flujo de entrada estándar (típicamente el teclado).

---
## Using namespace std
````javascript
std::cout << "Hola";
````
Es lo mismo que:
````javascript
using namespace std;
cout << "Hola";
````

---
## Main
La función main sirve como punto de partida para la ejecución del programa. 
````javascript
int main(){
    
}
````

---
## Escribir
En pseudo código:
````javascript
Escribir "Hola Mundo!"
````
En C++:
````javascript
cout<<"Hola Mundo!"<<endl;
````

---
## Leer
En pseudo código:
````javascript
Leer num1
````
En C++:
````javascript
cin>>num1;
````

---
## Declarar variables
En pseudo código:
````javascript
Definir numEntero1, numEntero2, numEntero4 Como Entero
Definir numComa4, numComa8, numComa9 Como Real
Definir letra como Caracter
Definir bandera como Logico
````
En C++:
````javascript
int numEntero2;
shor numEntero1;
long numEntero4;
float numComa4;
double numComa8;
long double numComa9;
char letra;
bool bandera;
````

---
## Code Blocks: Guardar
Es MUY IMPORTANTE incluir la extension ".cpp"
![Code Blocks](images/U3_programacion/code_blocks_2.png)

---
## Code Blocks: Build and Run
![Code Blocks](images/U3_programacion/code_blocks_3.png)

---
#### Comenzando con un nuevio lenguaje...
![Comenzando con un nuevo lenguaje](images/U3_programacion/lets-compile.png)

---
## A tener en cuenta...
* Guardar con extensión **.cpp**
* Emplear **;** al final de cada oración
* Realizar un **build & play** si se realizaron cambios

---
## Errores más comunes
<!-- .slide: style="font-size: 0.8em" -->
* Omitir un punto y coma **;** al final de una sentencia.
* Omitir la declaración de una variable.
* Escribir mal la directiva **#include**
* Escribir mal el nombre de alguna biblioteca añadida con la directiva **#include** (Ej. <iostream>)
* Confundir **=** con **==**
* Escribir el operador **!=** distinto al revés **=!**
* Escribir los operadores **>=** y **<=** al revés **=<, =>**
* No emplear bien los paréntesis y llaves
* Confundir los separadores del **cin** y **cout**
    * cin **>>** ingresar_var;
    * cout **<<** "Mostrar el valor de " **<<** ingresar_var **<<** endl;

---
## Confundir = con ==
<!-- .slide: style="font-size: 0.7em" -->
Hay que tener mucho cuidado con esto, el programa compilara, pero el comportamiento del programa no es el que esperamos:
* **=** significa **Asignación**, sirve para dar valor a una variable:
    * int numero_entero = 3;
    * bool flag = true;
* **==** es un operador de comparación, devolverá verdadero cuando las expresiones a la derecha y a la izquierda valgan lo mismo, 
y falso en otro caso:
    * if(a == b) {...} **true** si a y b tienen el mismo valor almacenado, **false** en otro caso.
    * if((a>3) == (c<4)){...} **true** si a es mayor que 3 y c es menor que 4 simultáneamente, **falso** en otro caso
    * if(a == 3){...} **true** si a tiene almacenado el valor 3, **falso** en otro caso.


---
## Ejercicios
Resuelve nuevamente los ejercicios del **[Trabajo Practico I](https://ucc-fundamentosprogramacion.github.io/GTP/TP1_ejercicios.html#/1): Estructura Secuencial**, del 1 al 14 

---
## Librerias o Bibliotecas
Archivos que podemos incluir o importar en nuestro programa.

Estos archivos contienen especificaciones de diferentes funcionalidades ya construidas y utilizables que podemos
agregar a nuestro programa
````javascript
#include <cmath>
````

---
## [cmath](http://www.cplusplus.com/reference/cmath/)
<!-- .slide: style="font-size: 0.8em" -->
Contiene algunas funcionalidades como:
* atan: arco tangente **atan(double x)** x en radianes
* pow: potencia. **pow(double base, double exponente)**
* sqrt: raiz cuadrada **sqrt(double x)**
* abs: valor absoluto **abs(double/float x)**
* sin: seno **sin(double/float x)** x en radianes
* cos: coseno **cos(double/float x)** x en radianes
* tan: tangente **tan(double/float x)** x en radianes

Tambien constantes:
* M_PI

---
## Ejercicios
Resuelve nuevamente los ejercicios del **[Trabajo Practico I](https://ucc-fundamentosprogramacion.github.io/GTP/TP1_ejercicios.html#/1): Estructura Secuencial**, del 15 al 22 

---
## ¿Dudas, Preguntas, Comentarios?
![DUDAS](images/pregunta.gif)
