---
title: 11-Transformaciones Lineales
---

La **transformacion lineal** se podria definir como una funcion, que nos permite comparar diferentes espacios vectoriales.

## Definicion

Imaginemos que tenemos $V$ y $W$ dos $K$-espacios vectoriales reales y $T : V arrow.r W$ **una funcion**.

Tambien tenemos los vectores $u,v in V$

$T$ es una **transformacion lineal** si:

1. $T(u+v) = T(u) + T(v)$, tiene la suma.

2. $T(lambda v) = lambda T(v)$, tiene la multplicacion.

### Ejemplos

- $T : RR^2 arrow.r RR^2$, $T(x,y) = T(x,0)$, esto serian todos los puntos en el eje $x$.

- $T : RR^3 arrow.r RR^3$, $T(x,y,z) = T(x,y,0)$, esto seria lo mismo que antes pero todos los **planos** del eje $x,y$

- $T : #strong[Mat]$$(RR)_(m times n)  arrow.r #strong[Mat]$$(RR)_(m times n)$, $A$ es una matriz $n times m$, T(A) = A^t, esta es una transformacion para hacer la matriz **transversa**.

- Tambien se puede hacer la derivada de un polinomio $T(p(x)) = p(x) prime$, entre muchas otras funciones comunes.

### Propiedades

1. Si nosotros tenemos una transformacion lineal **no importa** desde que espacio a que espacio este yendo, si nostros le pasamos el **vector 0**, vamos devolver el vector **0** del espacio de llegada.

$$
T(0_v) = 0_w;
$$

Con $V$ y $W$ siendo subespacios.

2. Si nosotros pasamos un vector negativo, o que este siendo multiplicado por un *escalar* $lambda$ negativo por ejemplo $T(-v)$, este va a devolver un **vector transformado** que va a estar siendo multiplicado por $-1$.

$$
T(-v) = -w
$$

3. Preservacion de combinaciones lineales, ejemplo:

$$
T(lambda v_1 + alpha v_2 + dot dot dot + beta v_n) = lambda T(v_1) + alpha T(v_2) + dot dot dot +beta T(v_n)
$$

### Ejemplos de Transformaciones triviales

- Si tenemos $T(v) = 0$, esta es conocida como **transformacion 0 o transformacion nula**, basicamente asigna el vector de $V$ a **vector nulo** en $W$

- Otro ejemplo es $T(v) = v$ y este te devuelve la identidad es decir el mismo vector pero representado en el otro espacio.

>[!note]
> Si tenemos una base $B$ de un espacio $V$, y ademas tenemos dos transformacion lineal definidas como $T: V arrow.r W; S: V arrow.r W$, cualquier $v in V$ va a cumplir que $T(v) = S(v)$ si **la base** tambien lo cumple $T(B_i) = S(B_i)$ ($B_i$ es un vector cualquiera de la base).

### Teorema

Se dice que cualquier vector **de la base** de $V$, en una transformacion **siempre** tiene un **vector de unico de llegada** en $W$. 

Por lo tanto la unica manera de que esa transformacion de lo mismo que la otra es que tengan la **misma base**

### Ejercicio Parcial

![EjTrans1](2025-02-17_01-11.png)

Primero nos damos cuenta que si hacemos los pasos para sacar la base del subespacio que nos dan $S_2$ podemos verificar con la combinacion lineal.

$$
p(-1) = -a + b -c + d
$$
$$
$$
$$
d = a -b + c
$$

Las condiciones para armar el polinomio base las tenemos ahi y es que $d = a -b + c$.

$$
a x^3 + b x^2 +c x + a -b + c = a (x^3 + 1) + b (x^2 -1) + c (x +1) 
$$

Ahora tenemos la base ${x^3 +1, x^2 -1, x+1}$.

Con esto nos podemos dar cuenta que en realidad la transformacion lineal va a ser **unica porque la transformacion lineal de una base es unica**. Con esto en mente ya descartamos 3 posibilidades.

Ahora falta confirmar cual es el resultado del poliniomio que pasa por la transformacion.

Al nosotros saber **como es la base**, la podemos usar para **encontrar las coordenadas** y usar los valores que nos da la transformacion lineal.

$$
x^3+2x+3 = lambda (x^3+1) + alpha (x^2-1) + beta (x+1)
$$
$$
$$
$$
x^3 + 2x + 3= lambda x^3 + alpha x^2 + beta x
$$

Si nos damos cuenta y **agarramos los coeficientes** $lambda = 1; alpha = 0; beta = 2$

Asi que $(x^3+1) + 2(x+1)$ ahora podemos resolver cuanto da ya que segun la transformacion $T(x^3 +1) = x +1$ y $T(x+1) = x^2 + x$

$$
x+1 + 2(x^2 + x) = 2x^2 + 3x + 1
$$

Como nos damos cuenta la **opcion correcta es la** $C$











