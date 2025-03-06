---
title: 8-Rango de una matriz
---

## Rango de una matriz

Imaginemos que tenemos dos matrices $A$ y $B$, de un tamano $n times m$, si $A$ y $B$ son equivalentes (**o sea las filas de $A$ son combinacion lineas de las filas de $B$ y viceversa**) por filas o columnas, entonces el espacio vectorial fila o columna de $A$ es igual al espacio fila o columna de $B$.

Parar tener un ejemplo mas claro de un espacio fila aca esta un ejemplo:

$$
A = mat(a,b;c,d)
$$
$$
$$
$$
F = {(a,b),(c,d)}
$$

Y ahora uno del espacio columna

$$
C = {(a,c),(b,d)}
$$

---

Tambien tenemos que si $A prime$ (la matriz escalarizada $A$), entonces el **espacio fila** de $A$ es igual a el de $A prime$.

Entonces el conjunto de vectores fila (no nulos) de $A prime$ forma un conjunto **linealmente independiente** que a la vez es una base de del **espacio fila** $A prime$, y segun la proposicion anterior siginifica que tambien es una **base del espacio fila** de $A$

Cabe aclarar que el rango de la matriz escalarizada es tambien **la dimension que tiene el espacio fila**. 

### Teorema

Sea una matriz $A$ el **Rango(A)** es **igual a la dimension del espacio fila y columna**

### Ejercicios parcial

### 1)
![Rej1](2025-02-09_22-15.png)

En estos casos si queremos saber si el conjunto es linealmente independiente formamos una matriz con el conjunto. Para luego hacerle **el determinante**.

$$
A = mat(0,-1,1;k,1,-2;-4,k,0)
$$

El $det(A) = k^2 - 4$, la afirmacion que nos piden verificar es si **es linealmente independiente** solo si $k eq.not 2$, la solucion es tan facil como ver que $k = |sqrt(4)| arrow.r.double.long k = |2|$, por lo tanto **acepta dos valores**, asi que es **linealmente independiente** si $k eq.not 2$ y $k eq.not -2$.

En conclusion la afirmacion es **falsa**.

### 2)
![Rej2](2025-02-09_22-28.png)

En este ejercicio primero tendriamos que **escalarizar la matriz**, y nos quedaria asi:

$$
mat(1,1,5;0,2,2;0,0,t+2)
$$

Ya por esto nos damos cuenta que la opcion $C$ cuenta con que si $t=-2$ basicamente el rango de $A =2$, ademas es tan facil como verificar que en efecto **es combinacion lineal de las otras filas la tercera**. Dandonos los valores $lambda = 0;alpha = -1$






