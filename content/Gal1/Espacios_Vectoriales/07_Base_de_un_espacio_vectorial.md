---
title: 7-Base de un espacio vectorial
---

Para empezar la definicion de una base se puede expresar asi:

Supongamos que tenemos un **E.V** llamado $V$ y $B subset V$.

Decimos que $B$ es una **base** de $V$ si cumple:

1. $[B] = V$
2. $B$ es linealmente independiente

>[!important] Afirmacion
>Si $B = {v_1,v_2, dot dot dot, v_n}$ es una **base** de un espacio vectorial $V$ entonces **cualquier conjunto de vectores** que este en $V$ y tenga una **cantidad de elementos mayor** a $n$, significa que es **linealmente dependiente**.
>
>Tambien si tenemos **dos bases** de un mismo **E.V** $B_1$ y $B_2$ las dos tienen que tener la misma cantidad de elementos.

### Ejemplos de bases

1. $V = RR^2, dim(V) = 2$. Tenemos la **base canonica** $B_c = {(1,0),(0,1)}$ y una base cualquiera $B = {(2,3),(-1,2)}$
2. $V = RR^3, dim(V) = 3$. Tenemos la **base canonica** $B_c = {(1,0,0),(0,1,0),(0,0,1)}$ y una base cualquiera $B = {(1,1,0),(1,-1,0),(0,0,1)}$
3. $V = R_2 [x], dim(V) = 3$. Tenemos la **base canonica** $B_c = {1,x,x^2}$ y una base cualquiera $B = {1+x,x-x^2,1+x^2}$

### Extraer una base de un subespacio

Imaginemos que tenemos a $W = {(alpha, space beta - alpha, space beta) : alpha, beta in RR}$ un subconjunto de $RR^3$. Es claro que $W$ es un subespacio de $RR^3$.

Encontraremos ahora una base de este:

$$
(alpha, space beta - alpha, space beta) = (0,beta, beta) + (alpha, -alpha,0) = beta(0,1,1) + alpha(1,-1,0)
$$

Por lo tanto **una base de** $RR^3$ es $B = {(0,1,1),(1,-1,0)}$ y es linealmente independiente.

### Importancia de las bases en los espacios vectoriales

Bueno un resumen de la importancia de las bases en varios puntos seria asi:

>[!note] Grimario
> $n = dim(V)$
> 
> Y siempre se hablando en base a $V$

1. Cualquier conjunto **linealmente independiente** con $n$ vectores es una base.
2. No existen conjuntos **linealmente independientes** con mas de $n$ vectores.
3. No existen conjunto que **generen a** $V$ con menos de $n$ vectores.
4. Cualquier subespacio tiene **dimension igual o menor** que el espacio vectorial al que pertenece.

---

Imaginemos que tenemos dos conjuntos $U$ **linealmente independiente** y $G$ un conjunto generador de $V$.

Claramente $U,G subset.eq V$.

- Si $U subset.eq G$, es decir esta incluido un conjunto **linealmente independiente** en un **generador**, es claro que hay una base que los contiene a los dos, ya que la **base es linealmente independiente y un generador a la vez**,  $ space U subset.eq B subset.eq G$

- $U$ esta contenido en una base de $V$ y $G$ contiene una base de $V$, asi va la jerarquia como se muestra arriba.

- El numero de elementos de $U lt.eq G$, por lo tanto la jerarquia seria asi $|U| lt.eq |B| lt.eq |G|$.

## Ejercicios de parcial (Del tema recien dado)

### 1)

![Ejepa1](2025-02-05_03-14.png)

Bueno, tenemos dos conjuntos, el primero es el conjunto $L$ que si lo "investigamos" nos vamos a dar cuenta de que es **linealmente independiente** y genera un espacio de **dimension 3**.

Al pasarlo a una matriz nos queda asi:

$$
mat(1,1,1;0,1,1;0,0,1)
$$

Como se puede ver es una **base de** $RR_2 [x]$. 

Luego como podemos ver hace **una union** con otro cojunto y nos preguntan cuantas bases existen de $RR_3 [x]$ tal que $L subset.eq B subset.eq G$, o sea que $L$ esta incluido en $B$ y $B$ esta incluido en $G$.

Como podemos ver $L$ solo genera 0 bases de $RR_3 [x]$ pero si lo unimos con el otro conjunto es decir:

$$
L union {x^3} = mat(1,1,1,0;0,1,1,0;0,0,1,0;0,0,0,1)
$$
$$
$$
$$
L union {x^3+x^2}= mat(1,1,1,0;0,1,1,0;0,0,1,1;0,0,0,1) 
$$
$$
$$
$$
L union {x^3+x^2+x} =mat(1,1,1,0;0,1,1,1;0,0,1,1;0,0,0,1)
$$

Como podemos ver siempre que anadimos uno de estos vectores nos damos cuenta que no modfica si es **linealmente independiente** el conjuntoy tampoco afecta al **rango**.

Por lo tanto genera **3 bases distintas**.

### 2)

### 3)

![Ejepa3](2025-02-07_22-34.png)

