---
title: 4-Subespacios generados por conjuntos de vectores
---

## Introduccion 

Supongamos que tenemos un **E.V** llamado $V$ y tenemos un **S.V** llamado $S$, en pocas palabras en esta seccion queremos **encontrar el subespacio mas simple** que contenga a $S$, pero que tambien este **incluido** en $V$.

## Explicacion y ejemplo

### Combinacion Lineal y Definicion

Decimos que un vector $v$ es una **combinacion lineal** de los vectores $v_1, v_2, dot dot dot, v_n$ si existen los escalares/coordenadas tales que $lambda_1, lambda_2, dot dot dot, lambda_n$ y 

$$
v = lambda_1 v_1 + lambda_2 v_2 + dot dot dot + lambda_n v_n
$$

Si $S$ es un subconjunto (no vacio) del **E.V** $V$, vamos a llamarle $[S]$ al conjunto de los vectores de $V$ que pueden ser expresados como una **combinacion lineal** de los vectores de $S$.

En el caso que $S = {v_1, v_2, dot dot dot, v_n}$

$$
[S] = {w in V : w = lambda_1 v_1 + lambda_2+ v_2 + dot dot dot + lambda_n v_n, space v_i in S, space lambda in RR, space n in NN}
$$

Podemos ver que **cada elemento** de $[S]$ es una **combinacion lineal** de un numero **finito** de elementos de $S$.

A todo esto el subespacio $[S]$ es el subespacio de $V$ **mas chico que contiene** a los elementos de $S$. 

Lo llamaremos el **espacio generado** por $S$

> [!tip] Teorema
> Si tenemos un espacio vectorial y un subconjunto $S$ de $V$ no vacio. Entonces $[S]$ es un subespacio de $V$.

### Ejemplos

Tenemos dos vectores de $RR^3$, $v = (1,2,3)$ y $w = (-1,2,-2)$ entonces el menor subespacio que contiene a $v$ y $w$ es:

$$
[{v,w}] = {(lambda_1 v + lambda_2 w : lambda_1, lambda_2 in RR)} = {lambda_1 (1,2,3) + lambda_2(-1,2,-2):lambda_1, lambda_2 in RR }
$$

Esto se puede simplificar como:

$$
[{v,w}] = {lambda_1 - lambda_2, 2 lambda_1 + 2 lambda_2, 3 lambda_1 - 2 lambda_2 : lambda_1, lambda_2 in RR }
$$

Basicamente se podria decir que $(x,y,z) in [S]$ si cumple las siguientes condiciones:

$$
lambda_1 - lambda_2 = x
$$
$$
$$
$$
2 lambda_1 + 2 lambda_2 = y
$$
$$
$$
$$
3 lambda_1 - 2 lambda_2 = z
$$

Algo a observar es que estas condiciones que recien logramos sacar del conjunto, **las podemos llevar a ser algo mas**, como un plano o una recta. Esas mismas condicones **se pueden pasar para ser una matriz**.

Si vemos bien pasamos los coeficientes de los $lambda_1$ y $lambda_2$ en cada situacion a una matriz.
$$
mat(1,-1,x;2,2,y;3,-2,z; augment: #2) arrow.r.double.long mat(1,-1,x;0,4,y-2x;0,0,z+(-y-10x)/4; augment: #2)
$$

Luego de escalarizarla abajo del todo nos queda que

$$
0 = z+(-y-10x)/4
$$

Vamos a dejarlo un poco mas lindo multiplicando a todo $times 4$

$$
0 = 4z-y-10x
$$

Como podemos observar **esto es un plano**, por lo tanto se podria decir que el subespacio generado por esos dos vectores $w$ y $v$ es el plano
$4z-y-10x$

## Definicion generador

Digamos que tenemos el **E.V** llamado $V$ y el **S.V** de $V$ llamado $S$, decimos que $W$ un subconjunto de $S$ es un generador de $S$ si $[W]= S$. 

En otras palabras, $W$ es un generador de $S$ si cada elemento de $S$ puede ser expresado **como una combinacion lineal** de elementos de $W$.


## Primer ejemplo
Imaginemonos el **E.V** $V = RR^3$

### a)

Tenemos el conjunto definido como $W$
$$
W = {(1,0,0), (0,1,0), (0,0,1)}
$$

En este caso cualquier vector de $[W]$ tiene la forma $a (1,0,0) + b (0,1,0) + c (0,0,1)$ donde $a,b,c$ numeros reales $RR$ y representan los $lambda$ de antes.

> [!note] Aclaracion
> Basicamente el conjunto $[W]$ le pone un formato al conjunto.
> Por poner un ejemplo: $a (1,0,0) + b (0,1,0) + c (0,0,1)$, el conjunto es el $W$ y le puso los $a,b,c$ que podrian ser mas.

Por lo tanto este subespacio se podria poner como:
$$
[W] = {(a,b,c) in RR^3 : a,b,c in RR} = RR^3
$$

Asi el espacio que genera $W$ es todo $RR^3$, lo que nos deja como conclusion que $W$ es un conjunto generador de $RR^3$

### b)

$$
W = {(1,0,0), (0,1,0), (0,0,0)}
$$

Basicamente este conjunto no genera todo $RR^3$, pero seria bastante acorde decir que genera $2/3$ de $RR^3$.

Si le queremos dar "formato" de **combinacion lineal** hacemos esto.
$$
[W] = [{(1,0,0),(0,1,0)}] = {(a,b,0) in RR^3 : a, b in RR}
$$

En este caso le pusimos el formato $a(1,0,0) + b(0,1,0)$

### c)

$$
W = {(1,2,3),(0,1,-1),(2,4,4)}
$$

Queremos saber si $W$ genera $RR^3$ por lo tanto vamos a ver si podemos expresar cualquier vector $(x,y,z)$ como combinacion lineal de los vectores de $W$.

Asi que vamos a plantearlo asi:

$$
lambda(1,2,3) + alpha(0,1,-1) + beta(2,4,4) = (x,y,z)
$$

Donde lambda, alpha y beta son los escalares **que queremos determinar**.

Agrupando las cordenadas podemos hacer un sistema con las mismas.
$$
 cases(
    lambda + 2beta = x \
    2lambda + alpha + 4beta = y \
    3lambda - alpha + 4beta = z
  )
$$
 
Si resolvemos el sistema vamos a encontrar los valores de $lambda, alpha$ y $beta$ que nos permiten generar cualquier vector $(x,y,z)$

$$
lambda = -9x + 2y + 2z
$$
$$
$$
$$
alpha = -7x + 2y + z
$$
$$
$$
$$
beta = 5x - y - z
$$

Que haya dado este resultado nos dice que cualquier vector de $RR^3$ puede **ser expresado como combinacion lineal** usando los escalares que ya nos dieron.

En resumen el conjunto $W$ genera todo el espacio de $RR^3$ y para **averiguar las coordenadas(o el valor de cada escalar)**, deberiamos de **resolver el sistema como una matriz**.

## Segundo ejemplo

Consideremos el **E.V**  $V = #strong[Mat]$$(RR)_(2 times 2)$

Tenemos el conjunto $S = {mat(1,0;0,0),mat(0,1;1,0),mat(0,0;0,1)}$ y queremos **determinar** el espacio generado por $S$, es decir $[S]$.

Nos podemos dar cuenta que el conjunto $[S]$ **genera el espacio de las matrices simetricas** $A in #strong[Mat]$$(RR)_(2 times 2)$ tal que $A^t = A$. Lo podriamos definir asi:

$$
[S] = {A = mat(a,b;b,c), space a,b,c in RR}
$$

Ademas el conjunto $S_1 = {mat(1,0;0,1),mat(1,0;0,-1),mat(0,1;1,0)}$ tambien genera el mismo subespacio que $S$. 

La razon es que **cualquier matriz simetrica se puede expresar como combinacion lineal** de las matrices de $S_1$ de la siguiente manera:

$$
A = (a+c)/2 mat(1,0;0,1) + (a-c)/2 mat(1,0;0,-1),b mat(0,1;1,0)
$$

> [!note]- Aclaracion
> La explicacion de porque aparece $(a+c)/2$ es porque aparece otra matriz $mat(1,0;0,-1)$ que cambia el valor de los escalares.
> En este caso seria asi: $mat(lambda + alpha, beta; beta, lambda-alpha) = mat(a,b;b,c)$. Nos da que $a+c = 2lambda$, **por lo tanto** $lambda = (a+c)/2$
> 
> La explicacion completa y mas entendible se puede encontrar en este [link](https://chat.deepseek.com/a/chat/s/0baa86f9-42a8-4478-9b77-469509468e06)

## Tercer ejemplo

Tenemos el **E.V** $V= RR_2 [x]$, y el conjunto $S = {1,x,x^2}$

En este caso el conjunto $S$ **es un generador del espacio vectorial** $V$.

$$
[S] = lambda dot 1 + alpha x + beta x^2
$$


> [!tip] Observacion
>  El subespacio **mas chico** de la union $U union V$ que vendria a ser $[U union V]$, si bien la **union no genera otro subespacio**, podriamos decir que $[U union V] = U + V$
> Que en ese caso si genera un subespacio.

---

## Dato curioso

Supongamos que tenemos un **E.V** llamado $V$ y un conjunto **finito** de vectores ${v_1, v_2, dot dot dot, v_n}$ de $V$. Si alguno de los vectores, por ejemplo $v_2$ es una **combinacion lineal** de los demas $(n - v_2)$ vectores, entonces lo espacios generados por el conjunto ${v_1, v_2, dot dot dot, v_n}$ y el conjunto ${v_1, v_3, dot dot dot, v_n}$ es decir sin el vector $v_2$ son iguales.

Por lo tanto la **cantidad de combinaciones lineales que generan son las mismas**:

$$
[{v_1, v_2, dot dot dot, v_n}] = [{v_1, v_3, dot dot dot, v_n}]
$$
