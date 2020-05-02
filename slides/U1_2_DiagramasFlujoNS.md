---
title: Fundamentos de la Programación
theme: sky
slideNumber: true
---

# Diagramas de Flujo y N-S
<small>
Created by <i class="fab fa-telegram"></i>
[edme88]("https://t.me/edme88")
</small>

---
## Diagramas de Flujo
¿Qué les parece que es un diagrama de flujo?

¿Cómo lo definirían con sus palabras?
    
---
## Diagrama de Flujo
Representa la esquematización gráfica de un algoritmo.

Muestra gráficamente los pasos o procesos a seguir para alcanzar la solución de un problema.
    
A partir del mismo se escribe un programa en algún lenguaje de programación.

---
## Diagrama de Flujo
* Se utilizan símbolos (cajas) estándar que representan los pasos del algoritmo
* Unidos por flechas: líneas de flujo
* Los símbolos están normalizados

---
### Simbolos de Diagrama de Flujo
<!-- .slide: style="font-size: 0.8em" -->
| Simbolo | Explicación |
|---------|-------------|
| ![Inicio-Fin](images/U1_resolucion_problemas/sim_inicio-fin.png) | Marcar el inicio y el fin del diagrama de flujo. |
| ![Lectura](images/U1_resolucion_problemas/sim_lectura.png) | Introducir los datos de entrada.  Expresa lectura. |
| ![Asignacion](images/U1_resolucion_problemas/sim_asignacion.png) | Expresa procesos: asignaciones, operaciones aritméticas, cambios de valor de celdas en memoria, etc |

---
## Simbolos de Diagrama de Flujo
<!-- .slide: style="font-size: 0.8em" -->
| Simbolo | Explicación |
|---------|-------------|
| ![Si-No](images/U1_resolucion_problemas/sim_si-no.png) | Condición, dependiendo del resultado de la evaluación de la misma se sigue por una de las ramas o caminos alternativos. Se utiliza para if, while, do while. |
| ![sino](images/U1_resolucion_problemas/sim_sino.png) | Selectiva  doble si  entonces/sino. Condición. El resultado es verdadero se continúa por el camino de la Izquerda, y si es falso por el camino de la derecha. Se utiliza para if else. |

---
## Simbolos de Diagrama de Flujo
<!-- .slide: style="font-size: 0.8em" -->
| Simbolo | Explicación |
|---------|-------------|
| ![Decision Multiple](images/U1_resolucion_problemas/sim_decisionMultiple.png) | Representar una decisión múltiple.  En su Interior se almacena un selector, y dependiendo del valor de dicho selector se sigue por una de las ramas o caminos alternativos.  <br> Se utiliza para switch (case)|

---
## Simbolos de Diagrama de Flujo
<!-- .slide: style="font-size: 0.8em" -->
| Simbolo | Explicación |
|---------|-------------|
| ![Escritura](images/U1_resolucion_problemas/sim_escritura.png) | Representar la Impresión de un resultado.  Expresa escritura. |
| ![Fechas](images/U1_resolucion_problemas/sim_flechas.png) | Expresar la dirección del flujo del diagrama |
| ![Conexion](images/U1_resolucion_problemas/sim_conexion.png) | Expresar conexión dentro de una misma página |

---
## Simbolos de Diagrama de Flujo
<!-- .slide: style="font-size: 0.8em" -->
| Simbolo | Explicación |
|---------|-------------|
| ![Conexion Paginas](images/U1_resolucion_problemas/sim_conexionEntrePaginas.png) | Expresar conexión entre páginas diferentes |
| ![Continuar](images/U1_resolucion_problemas/sim_continuar.png) | Expresar un módulo de un problema. Para continuar con el flujo normal del diagrama debemos primero resolver el subproblema que enuncia en su Interior |

---
## Diagrama de Flujo Básico
![Etapas Flow](images/U1_resolucion_problemas/etapas_flow.png)

---
### Diagrama de Flujo Básico
![Etapas Diagrama](images/U1_resolucion_problemas/etapas_diagrama_flujo.png)

---
![Entender Flow](images/U1_resolucion_problemas/understand_flow_chart.png)

---
### Reglas de DF
* Debe tener un inicio y un fin.
* Las líneas utilizadas para indicar la dirección del flujo del diagrama deben ser rectas, verticales y horizontales. (no inclinadas)
* Todas las líneas utilizadas para indicar la dirección del flujo del diagrama deben estar conectadas.
La conexión puede ser a un símbolo que exprese lectura, proceso, decisión, impresión, conexión o fin de diagrama.

---
### Reglas de DF
* El diagrama de flujo debe ser construido de arriba hacia abajo (top-down) y de izquierda a derecha (right to left). 
* La notación utilizada en el diagrama de flujo debe ser independiente del lenguaje de programación. 
* Es conveniente cuando realizamos una tarea compleja poner comentarios que expresen o ayuden a entender lo que hicimos. 

---
### Reglas de DF
<!-- .slide: style="font-size: 0.8em" -->
* Si el diagrama de flujo requiriera más de una hoja para su construcción, debemos utilizar los conectores adecuados y enumerar las páginas convenientemente.
* No puede llegar más de una línea a un símbolo.

![Regla 8](images/U1_resolucion_problemas/regla8.png)

---
### Diagramas N-S
Como el diagrama de flujo, pero se omiten líneas de flujo (flujo siempre es descendente) y las cajas son contiguas.
    
También conocido como diagrama de chaplin.

![Resolucion Problemas](images/U1_resolucion_problemas/s-n.png)

---
### Diagramas N-S
También es conocido como **Estructurograma**, ya que sirve para representar la estructura del programa.

Combina la descripción textual del pseudocódigo con la representación gráfica del diagrama de flujo

---
### Diagramas N-S: Caracteristicas
* En la primera caja va el **Inicio**
* La última instrucción es el **fin**
* Todas las declaraciones de variables y funciones se realizan bajo el inicio

---
### Diagramas N-S: Estructuras de Decision
![Condicion Doble](images/U1_resolucion_problemas/NS_condicion-doble.png)
![Condicion Multiple](images/U1_resolucion_problemas/NS_condicion-multiple.png)

* Doble
* Multiple

---
#### Diagramas N-S: Estructuras Iterativas
![Condicion Desde-Hasta](images/U1_resolucion_problemas/NS_condicion-desde-hasta.png)
![Condicion Hacer-Mientras](images/U1_resolucion_problemas/NS_hacer-mientras.png)
![Condicion Repetir-Hasta](images/U1_resolucion_problemas/NS_repetir-hasta.png)

* Desde-Hasta
* Hacer-Mientras
* Repetir-Hasta

---
![Miracle](images/U1_resolucion_problemas/miracle2.jpg)

---
## ¿Dudas, Preguntas, Comentarios?
![DUDAS](images/pregunta.gif)
