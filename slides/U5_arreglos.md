---
title: Fundamentos de la Programación
theme: black
slideNumber: true
---

# Arreglos
<small>
Created by <i class="fab fa-telegram"></i>
[edme88]("https://t.me/edme88") & 
<i class="fab fa-telegram"></i>
[rmarku]("https://t.me/rmarku")
</small>

---
<section>
## Arreglo
Conjunto de datos que se almacenan en memoria de manera contigua con el mismo nombre.

Para diferenciar los elementos de un arreglo se utilizan índices detrás del nombre del arreglo y encerrados por [].

---
## Arreglo
Colección finita, homogénea y ordenada de elementos.
    <ul>
* **Finita:** todo arreglo tiene un límite, es decirse debe determinar cuál será el número máximo de elementos que podrán formar parte del arreglo.
* **Homogénea:** todos los elementos de  un arreglo son del mismo tipo (todos enteros, todos reales, etc., pero nunca una combinación de distintos tipos). 
* **Ordenada:** Se puede determinar cuál es el primer elemento,  el segundo, el tercero,... y el n-ésimo elemento

---
## Arreglo 
![Arreglo Unidimensional](images/U5_arreglos/arreglo_unidimensional.png)

---
## Arreglo: Partes
* **Componentes:** Elementos que lo forman.
* **Índice:** Índice de elemento

![Arreglo Partes](images/U5_arreglos/arreglo_partes.png)

---
## Arreglo 
````javascript
int arr[3];
int arr[]={2,32,89};

````

---
## Arreglo: Operaciones
* Lectura/Escritura
* Asignación
* Actualización (inserción, eliminación, modificación)
* Ordenación
* Búsqueda

![Arreglo Partes](images/U5_arreglos/arreglo_partes.png)

---
## Operación: Lectura
Leer el valor de cada uno de sus elementos.

````javascript
int arr[]={3,4,6,7,8,9};

for(int i=0;i < 6; i++){
    cout<<arr[i]<<endl;
}
````

---
## Operación: Escritura
Escribir el valor de cada uno de sus elementos.

````javascript
int arr[5];

for(int i=0;i < 5; i++){
    cin>>&arr[i];
}
````

---
## Operación: Asignación
No es posible asignar directamente un valor a todo el arreglo, sino que se debe asignar el valor deseado a cada componente.

---
## Tipo de Arreglos
* **Unidimensionales o Lineales:** Cualquier elemento es referenciado por un único  índice.
* **Multidimensionales:**  El número de dimensiones (índices) que se deben de utilizar en un arreglo depende del problema que debemos resolver

---
## ¿Dudas, Preguntas, Comentarios?
![DUDAS](images/pregunta.gif)