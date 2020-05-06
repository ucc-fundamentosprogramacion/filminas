---
title: Fundamentos de la Programación
theme: sky
slideNumber: true
---

# Comenzar en C
<small>
Created by <i class="fab fa-telegram"></i>
[edme88]("https://t.me/edme88")
</small>

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
````javascript
Escribir "Hola Mundo!"
````
Es lo mismo que
````javascript
cout<<"Hola Mundo!"<<endl;
````

---
## Leer
````javascript
Leer num1
````
Es lo mismo que
````javascript
cin>>num1;
````

---
## Declarar variables
````javascript
int numEntero2;
float numComa4;
double numComa8;
char letra;
long numEntero4;
````

---
## Code Blocks: Guardar
![Code Blocks](images/U3_programacion/code_blocks_2.png)

---
## Code Blocks: Build and Run
![Code Blocks](images/U3_programacion/code_blocks_3.png)

---
## A tener en cuenta...
* Guardar con extensión **.cpp**
* Emplear **;** al final de cada oración
* Realizar un **build & play** si se realizaron cambios

---
## ¿Dudas, Preguntas, Comentarios?
![DUDAS](images/pregunta.gif)
