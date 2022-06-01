---
title: Fundamentos de la Programación
theme: sky
slideNumber: true
---

## Programación Modular

Created by <i class="fab fa-telegram"></i>
[edme88](https://t.me/edme88)

---
### Funciones
Una **función** es un conjunto de sentencias, con un nombre común, que se pueden llamar desde cualquier parte de un programa.
Se pueden reutilizar una o más veces reduciendo repeticiones.

En C/C++ todas las funciones son globales, es decir, se pueden llamar desde cualquier punto del programa

---
### Funciones
Permiten dividir un proyecto grande en módulos pequeños y manejables, donde cada función realice una tarea determinada.

Cuando se ejecuta la sentencia **return** o termina el código de la función, se retorna al punto en que fue llamada por el programa.

---
### Estructura de una Función
```cpp
tipo_de_retorno nombre_funcion(lista_de_parametros_formales){
    "cuerpo de la función";
    return expresión;
}
```

* **tipo_de_retorno:** <sub><sup>Tipo de valor devuelto por la función o la palabra reservada **void** si la función no devuelve ningún valor </sup></sub>
* **nombre_funcion:** <sub><sup>Identificador o nombre de la función. </sup></sub>
* **lista_de_parametros_formales:** <sub><sup>Lista de declaraciones de las parámetros de la función separados por coma.</sup></sub>
* **expresión:** <sub><sup>valor que devuelve la función</sup></sub>

---
### Ejemplo: Función
```cpp
float producto(float num1, float num2){
    float pro;
    pro = num1*num2;
    return pro;
}
```

---
### Ejemplo: Uso de Función
````cpp
#include <iostream>
using namespace std;

float producto(float num1, float num2){
    float pro;
    pro = num1*num2;
    return pro;
}

int main(){
    float m,n, resultado;
    cout << "Ingrese 2 números"<<endl;
    cin >> m >> n;
    cout << "El producto es: " << producto(m, n);
}
````
---
### Prototipo de las Funciones
Se requiere que una función se declare o  defina antes de su uso. 
La **declaración** de una función se denomina **prototipo**. 

Un prototipo consta de: nombre_función(lista_parámetros_formales);

Los prototipos se situan normalmente al principio de un programa, antes del **main()**.

---
### Ejemplo: Prototipo
```cpp
#include <iostream>
using namespace std;

double promedio(double x1, double x2); //Prototipo

int main(){
    double med, numero1, numero2;
    
    cout << "Introducza 2 numeros: " << endl;
    cin >> numero1 >> numero2;
    
    med = promedio(numero1, numero2); //Llamada a la función
    cout << "La media es: " << med << endl;
}

double promedio(double x1, double x2){
    return (x1+x2)/2;
}
```

---
### Ejercicios
Resuelve los ejercicios del **[Trabajo Practico IV](https://ucc-fundamentosprogramacion.github.io/GTP/TP5_ejercicios.html#/1): Programación Modular** 

---
### Parámetros de una Función
Hay diferentes métodos para pasar variables(parámetros) a funciones:
* Parámetros por **valor** o por **copia**
* Parámetros por **referencia**
* Parámetros por **omisión** o **defecto**

---
### Parámetros por valor
La función recibe una copia de los valores de los parámetros actuales. 
La función receptora no puede modificar los parámetros de la función (parametro pasado).

---
### Parámetros por Valor
```cpp
void func_1(int y){
    cout << y << endl;
    y = y + 1;
    cout << y << endl;
    return y;
}

int main(){
    int x = 6;
    cout << x << endl; // 6
    func_1(x); // 6 y 7
    cout << x << endl; // 6
}
```

---
### Parámetros por Referencia o Dirección
Cuando la función recibe el parámetro pasado, devuelve el valor modificado a la función llamadora.

Al declarar los parámetros de la función, se debe agregar **&** posterior al tipo de dato, y emplear el mismo nombre de variable.

El valor se ve modificado porque se almacena en la misma dirección de memoria.

---
### Parámetros por Referencia o Dirección
```cpp
#include <iostream>
using namespace std;

void referencia(int& x);

int main(){
    int x = 20;
    cout << "Antes de la llamada " << x << endl; // 20
    referencia(x);
    cout << "Después de la llamada " << x << endl; // 23
}

void referncia(int& x){
    x += 3;
}
```

---
### Parámetros por Omisión o Defecto
Cuando se omite el argumento de un parámetro que es un argumento por defecto, se utiliza automáticamente este. 

Si se pasan valores a los argumentos omitidos, se utiliza ese valor.

La única restricción es que se deben incluir todas las variables desde la izquierda hasta el primer parámetro omitido.

---
### Parámetros por Omisión o Defecto
```cpp
#include <iostream>
using namespace std;
void caracteres(int cant, char car='*');

int main(){
    caracteres(4); // Imprime ****
    caracteres(8,'@'); // Imprime @@@@@@@@
}

void caracteres(int cant, char car){
    for(int i=0; i<cant; i++){
        cout << car;
    }
}
```

---
### Reglas de Argumentos por Defecto
* Los argumentos por defecto se deben pasar por valor.
* Los valores de los argumentos por defecto deben ser literales (no pueden ser variables).
* Después del primer argumento por defecto, los posteriores deben incluir valores por defecto.

---
### Ámbito o Alcance
El **ámbito** es la zona de un programa en la que es visible una variable.

Existen 4 tipos de ámbito:
* Programa
* Archivo fuente
* Función
* Bloque

---
### Ámbito: Programa
Estas variables pueden ser refernciadas por cualquier función en el programa completo.

Se las llama **variables globales**.

Se deben declarar al principio, fuera de cualquier función. 

---
### Ámbito: Archivo Fuente
Variable que se declara fuera de cualquier función y contiene la palabra reservada **static**.

Pueden referenciarse desde el punto en el que están declaradas hasta el final del archivo.

---
### Ámbito: Función
Esta variable se puede referenciar desde cualquier parte de la función.

Las variables declaradas dentro del cuerpo de una función, se dice que son **locales**.

---
### Ámbito: Bloque
Esta variable se puede referenciar desde cualquier parte del bloque, desde el punto donde está declarada hasta el final del bloque.

Las variables declaradas dentro del ámbito de una función tienen ámbito de bloque de la función.

---
### Ámbito: Ejemplo
```cpp
#include <iostream>
using namespace std;

float PI = 3.141592; // Ámbito de Programa o Ámbito Global
static int i; // Ámbito de Archivo Fuente

float perimetro_circulo(float r) {
    for(int j=0;j<10;j++){ // Ámbito de Bloque
        cout<<"Hola Mundo!!!"<<endl;
    }
    return PI * r * 2;    // r tiene ámbito de función
}

int main() {
    float r;    // Ambito de Función
    cout << "Ingrese un radio: ";
    cin >> r;

    cout << "El perimetro es " << perimetro_circulo(r) << endl;
}
```

---
## ¿Dudas, Preguntas, Comentarios?
![DUDAS](images/pregunta.gif)
