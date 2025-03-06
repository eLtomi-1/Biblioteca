---
title: Practico 9
---

Base y dimension

![P9ej1](2025-02-11_03-02.png)

**a)** Primero queremos hayar un generador y despues rezar para que sea **linealmente independiente**, asi que tratamos de sacar una variable para agarrar los vectores que lo generan.

$$
x + 2y - z = 0
$$
$$
$$
$$
z = x + 2y
$$ 

Ahora que ya sabemos **cuanto vale** $z$:

$$
(x, y, x + 2y) arrow.r.double.long x(1, 0, 1) + y(0,1,2)
$$

Si nos damos cuenta es **linealmente independiente** asi que es una base del subespacio $S$ con una dimension 2

**b)** Nesecitamos urgentemente plantear como serias los sitemas con $p(2) = 0$

$$
8a + 4b + 2c + d = 0 arrow.r.double.long d = -8a -4b -2c
$$

Por lo tanto si ahora lo aplicamos al polinomio base:

$$
a x^3 + b x^2 + c x -8a -4b -2c = 0 arrow.r.double.long a(x^3 -8) + b (x^2 -4) + c(x -2) =0
$$

Si lo pasamos a una matriz los vectores nos damos cuenta que es **linealmente independiente y ademas de una dimension 3**.

Asi que si es una base de un subespacio $S$, ${x^3 -8,x^2 -4, x -2}$.

**d)** En este tenemos que lograr hacer una matriz general que la suma de la diagonal sea **0**.

$$
mat(a,b;c,-a)
$$

Luego es tan facil como poner las variables como combinacion lineal.

$$
a mat(1,0;0,-1) + b mat(0,1;0,0) + c mat(0,0;1,0).
$$

Y sacar el conjunto que es una **base** ${mat(1,0;0,-1), mat(0,1;0,0), mat(0,0;1,0)}$

### 2)
![P9ej2](2025-02-11_22-34.png)

**a)** Lo primero de todo como ya sabemos que es un **generador** para pasarlo a una **base** nesecitamos hacerlo **linealmente independiente** asi que lo vamos a escalarizar en una matriz.

$$
mat(1,-1,2;4,-3,7;2,0,5;1,2,6) arrow.r.double.long mat(1,-1,2;0,1,-1;0,0,3;0,0,0) 
$$

Asi que el vector que sobra es el $(1,2,6)$.

**a)** Bueno en este caso hicimos lo mismo.

$$
mat(1,1,1,1;1,2,0,1;1,3,3,1;1,2,2,1;0,0,1,2) arrow.r.double.long mat(1,1,1,1;0,1,-1,0;0,2,2,0;0,-1,-1,0;0,0,1,2)
$$

Si nos damos cuenta el vector $mat(1,2,2,1)$ es el que perfectamente lo podemos restar y que quede en **0**

### 3)

![P9ej3](2025-02-12_02-44.png)

**a)** Bueno en este caso si armamos un sistema nos damos cuenta que alpha y beta son **0**

$$
 cases(
    alpha + beta = 0 \
    beta = 0 \
    2alpha = 0 \
    2alpha = 0
  )
$$

Aca sacamos lo que ya dijimos $alpha = 0; beta =0$ y ahora tenemos que anadir dos vectores mas para que genere un espacio de **dimension 4** y sea **linealmente independiente** a la vez.

Si lo planteamos como una matriz nos puede quedar asi:

$$
mat(1,1;0,1;2,0;2,0) arrow.r.double.long mat(1,1,0,1;0,1,0,0;2,0,0,0;2,0,1,0)
$$

Como podemos ver pusimos dos vectores mas ${(0,0,0,1),(1,0,0,0)}$, estos dos al ponerlos no afectan los valores de $alpha$ y $beta$ y ademas generan un espacio de **dimension 4**.

**b)** Aca tambien tenemos que hacer lo mismo y para resumir.

$$
mat(1,0;-1,1;1,-1;0,0) arrow.r.double.long mat(1,0,0,0;-1,1,0,0;1,-1,0,1;0,0,1,0)
$$

Metmimos estos dos vectores que cumplen ${(0,0,0,1), (0,0,1,0)}$, y traducido a poliniomios, ${x^3,x^2}$

### 4)

![P9ej4](2025-02-12_03-33.png)

**a)** Primero para probar que es una base, tenemos que saber si es **linealmente independiente** y si la **dimension coincide con el espacio**.

Para eso hacemos el **determinante al conjunto** y nos da que si **es linealmente independiente**, si bien nos falta la segunda parte que es que la **dimension sea la misma**, ahora averiguando las coordenadas nos vamos a enterar.

$$
mat(1,1,0,1;0,1,1,2;1,0,1,3; augment:#3) arrow.r.double.long mat(1,1,0,1;0,1,-1,1;0,0,2,2; augment:#3)
$$

Como nos podemos dar cuenta **el rango de la matriz es 3** asi que **si es una base**. Y ademas las cordenadas son $lambda=0;alpha=2;beta=1$

**b)** Ahora vamos a hacer exactamente lo mismo.

mat(2,1,2,4,1;0,0,3,-1,3;1,1,1,2,-4;0,0,5,2,6; augment:#4) arrow.r.double.long mat(2,1,2,4,1;0,1,0,0,-9;0,0,3,-1,3;0,0,0,11,3; augment:#4)

Como podemos ver, es **linealmente independiente**, genera una **dimension igual a la del espacio**, o sea **es base** y las cordenadas del vector son $lambda = 34/11; alpha = -0; beta =12/11; d = 3/11$

### 5) 
![P9ej5](2025-02-13_01-49.png)

Esta es bastante facil, tenemos que primero armar el sistema y pasarlo a matriz, y luego hacerle el determinante a esa matriz.

Armamos el sistema:

$$
lambda (1 + t) +  d (1+alpha t + t^2) + beta (1 + t^2) arrow.r.double.long (lambda + d + beta) + (d alpha + lambda) t + (beta + d) t^2
$$

Esto lo pasamos a matriz:

$$
A = mat(1,1,1;1,alpha,0;0,1,1) 
$$

El $det(A) = -alpha$ por lo tanto siginifica que depende de cuanto valga alpha si es **linealmente independiente o no**.

O sea si $alpha = 0$ es linealmente dependiente, asi que para que sea una base $alpha eq.not 0$ en resumen.

### 6)
![P9ej6](2025-02-13_21-27.png)

**a)** El rango de esta matriz es 2 y escalarizada queda asi:

$$
mat(1,2,3;0,-3,-6;0,0,0)
$$

La dimension del espacio ker **es igual** a $n$ que es la cantidad de columnas **menos el rango**.

Por lo tanto la dimension de ker es igual a $3-2 = 1$

Y **para verificar** la suma de la **dimension** de ker y **el rango** es $n$

$1+2 = n = 3$ 

**b)** Ahora hacemos lo mismo escalarizamos:

$$
mat(-2,4,-2,-4;0,-2,-5,-3;0,0,0,0)
$$

Tiene rango $2$ asi que la dimension del kernel es igual $4-2 = 2$ y para vericar $2 + 2 = n = 4$

**c)** Ahora hacemos lo mismo escalarizamos:

$$
mat(1,2,3,-4,8;0,0,-3,6,0;0,0,0,0,-7;0,0,0,0,0)
$$

$5-3 = 2$ y para verificar $2 + 3 = 5 = n$

### 7)
![P9ej7](2025-02-13_04-46.png)

**a)** Primero que todo queremos averiguar las bases de $S_1$ y $S_2$ asi que hacemos esto.

Para el primero sabemos que $x=z$.

$$
(x,y,x) = x(1,0,1) + y(0,1,0)
$$

Ahi tenemos la base de $S_1$, $B={(1,0,1)+(0,1,0)}$ y ahora la de $S_2$

$$
(x,y,0) = x(1,0,0) + y(0,1,0)
$$

Asi que $B_2 = {(1,0,0),(0,1,0)}$

Ahora queremos saber la base de $S_1 + S_2$ y $S_1 sect S_2$, para saber la interseccion, hacemos una interseccion entre las bases.

$$
B_1 sect B_2 = {(0,1,0)}
$$

Y para saber **la suma hacemos** la union y nos fijamos que sea linealmente independiente.

$$
B_1 union B_2 = {(0,1,0),(1,0,0),(1,0,1)}
$$

Y claramente como la interseccion no es nula la suma directa **no existe**.

**b)** Ahora vamos a exactamente lo mismo. 

Bueno primero agarrar las bases, el primer subespacio solo tiene $a x^2$ y el segundo tiene este $c x^2 + b x + c$.

Esto lo convertimos a esto:

$$
c (x^2 + 1) + b (x)
$$

Y el otro subespacio lo mismo.

$$
a (x^2)
$$

Asi que las dos bases son $B_1 = {x^2+1, x}$ y $B_2 = {x^2}$

Ahora hacemos la interseccion y nos da **que es nula**.

Y hacemos la **suma/union** nos queda esto {x^2, x^2+1, x} que si le hacemos la matriz nos da que es linealmente independiente y genera un espacio de dimension 3, por lo tanto es **una base**.

Como la interseccion es nula podemos confirmar que la **suma directa existe**

### 8)
![P9ej7](2025-02-14_02-42.png)

Ahora lo primero que queremos hacer es comprobar que la **union** de las bases es una base de $RR^4$.

Si escalarizamos los vectores de $B_1 union B_2$ nos da esto:

$$
mat(1,-2,1,1;0,0,-1,-5;0,0,-2,26; 0,0,0,-68)
$$

Es decir es linealmente independiente y encima genera el espacio $RR^4$ por lo tanto si es una base del espacio.

Y segundo la suma directa, claramente la suma directa no es porque la **interseccion** de las bases no es vacia $B_1 union B_2 = {(0,4,-1,1)}$
 



