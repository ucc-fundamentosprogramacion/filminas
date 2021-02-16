---
title: Fundamentos de la Programación
theme: sky
slideNumber: true
---

# Estructura de Control de Flujo Repetitivo o Iterativo
<!-- .slide: style="font-size: 0.8em" -->
<small>
Created by <i class="fab fa-telegram"></i>
[edme88]("https://t.me/edme88")
</small>

---
## Estructuras Repetitivas o Iterativas
Este tipo de estructura de algoritmos que permite repetir una o varias acciones un número determinado de veces 
se denominan BUCLES, LAZO o LOOP, y cada repetición del bucle se llama iteración o ciclo.

Todo bucle tiene que llevar asociada una condición, que es la que va a determinar cuándo se repite el bucle y cuando deja de repetirse.
   
---
## Construcción de Lazos o Ciclos
Frecuentemente debemos efectuar en programación cálculos recurrentes. Esta situación se presenta cuando una misma operación (o serie de operaciones) se debe repetir dentro de un programa.

La misma se resuelve mediante el empleo de lazos o ciclos de programación. Es decir repetir una serie de cálculos un número finito de veces.

---
## Lazos
Para la construcción de lazos se deben utilizar al menos un contador y una decisión. Con el contador se
van registrando la cantidad de veces que se realiza la repetición y con la decisión se determina cuando se debe finalizar.

---
![Flujo Ovejas](images/U2_control_flujo/flujo_ovejas.png)

---
## Contador
Es una variable que cuenta. Generalmente se inicializa en cero antes de incializar un ciclo.
````javascript
cont++
cont=cont+1
````

---
## Acumulador
Es una variable que almacena datos de una suma continua. 
Su característica más común es que su valor suele ser siempre una suma o resta del valor actual con un dato nuevo.
````javascript
acum=acum+nota
````

---
## Bandera
Es una variable tipo lógica que se incializa en VERDADERO ó FALSO.
Sirve para indicar que un determinado evento ocurrio.
````javascript
bandera=VERDADERO
bandera=true
````

---
![Warning](images/warning.png)

Bajo ninguna circunstancia hagas un loop infinito! LA COMPU VA A AUTODESTRUIRSE!!!

Bah, no es para tanto, pero nunca va a terminar el programa xD
   
---
## Tipo de Bucles
* While (mientras)
* Do While (hacer mientras)
* For (para)

---
## While
![While](images/U2_control_flujo/while.png)

---
## While
Esta estructura repetitiva “mientras”, es en la que el cuerpo del bucle se repite siempre que se cumpla una determinada condición.

````javascript
Mientras <cond> Hacer
    <acciones>
Fin mientraS
````

---
En las **acciones** suele haber alguna operación que afecte la condición (para llegar a una condición de corte).

---
## While: Ejemplo
````javascript
INICIO
    BOOLEANO tanqueLleno = falso
    MIENTRAS (tanqueLleno == falso)   HACER:
        llenar tanque
    FIN_MIENTRAS   // el tanque ya está lleno :)
FIN
````

---
## Trap While
[![Its a trap](images/U2_control_flujo/its_trap_flow.png)](https://www.youtube.com/watch?v=wk-6DPrcMv4#t=14s)

Si no hay condición de corte (si siempre se cumple el **condicional**) jamás se podrá salir del bucle.

---
## Ejercicios
Resuelve los ejercicios del **Trabajo Practico III: Diagramas de Flujo y Pseudocódigo de Estructuras Iterativas**, del 2 al 5 

---
## Do While
![Do While](images/U2_control_flujo/do_while.png)

---
## Do While
Esta estructura es muy similar a la anterior, sólo que a diferencia del while el contenido del bucle se ejecuta siempre al menos una vez, ya que la evaluación de la condición se encuentra al final.

De esta forma garantizamos que las acciones dentro de este bucle sean llevadas a cabo, aunque sea una vez independientemente del valor de la condición.

---
## Do While
````javascript
Repetir 
     <acciones>
Mientras Que <cond>
````

---
## Do While: Ejemplo
````javascript
INICIO
    BOOLEANO llegadaColectivo=false;
    REPETIR:
            esperar en la parada
    MIENTRAS (llegadaColectivo == false)
FIN
````

---
## Ejercicios
Resuelve los ejercicios del **Trabajo Practico III: Diagramas de Flujo y Pseudocódigo de Estructuras Iterativas**, del 6 al 9 

---
## For
![For](images/U2_control_flujo/for.png)

---
## For
Permite ejecutar un conjunto de acciones para cada elemento de una lista, o para cada paso de un conjunto de  elementos.

Suele emplearse cuando se conoce a priori la cantidad de ciclos.

---
## For
Podemos identificar tres componentes:
* inicialización
* condición de corte
* incremento

---
## For
````javascript
Para varX=<valor_inicial> Hasta <valor_final> Con Paso <paso> Hacer
    <acciones>
Fin Para
````

---
## For: Ejemplo
```javascript
INICIO
    PARA RUEDA=1 Hasta 4 Con Paso 1 Hacer
        Escribir "Inflar Rueda"
    FIN_PARA 
FIN
```

---
## Ejercicios
Resuelve los ejercicios del **Trabajo Practico III: Diagramas de Flujo y Pseudocódigo de Estructuras Iterativas**, del 10 al 18 

---
### Qué tengo que escribir eso en el pizarron 500 veces?
No hay problema profe!
![Joke For](images/U2_control_flujo/joke_for.jpg)

---
## Ejercicios
Resuelve los ejercicios del **Trabajo Practico III: Diagramas de Flujo y Pseudocódigo de Estructuras Iterativas**, del 19 al 42 

---
## ¿Dudas, Preguntas, Comentarios?
![DUDAS](images/pregunta.gif)
