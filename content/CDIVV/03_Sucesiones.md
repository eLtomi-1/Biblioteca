---
title: 3- Sucesiones
---

## Definicion

Una sucesion de **numeros reales** es una funcion $a:NN arrow RR$

Hablando de **notacion** lo denotamos como el **objeto entero** a $(a_n)_(n in NN)$ si queremos agarrar un elemento del objeto usariamos $a_3$ por poner un ejemplo.

Para que nos hagamos una idea vamos a poner un **ejemplo una sucesion**:

$$
a_n = 1 space forall n in NN
$$

Esta lista todas las sucesiones es decir $a_1, dot dot dot, a_n = 1$ asi que esta es una facil.

>[!important]
> Un dato curioso es que por mas que los conjuntos imagenes sean **iguales** estamos igualmente perdiendo mucha informacion de la sucesion, como por ejemplo.
>
> Tenemos una sucesion $1,0,1,1,1$ y otra que es $0,0,0,0,1$ y las dos tienen el conjunto $"Im"(a_n) = {0,1}$ y sin embargo son totalmente distintas.

Seguimos con los ejemplos:

1. $a_n = (-1)^n$

Esta va a ir variando entre $1$ y $-1$.

2. $a_n = 1/n$

Esta va a ser $1,1/2,1/3,1/4 dot dot dot$

3. $a_n = n$

Un poco redundante pero esta seria $1,2,3,4,5 dot dot dot$


## Sucesiones acotadas

Decimos que una sucesion es acotada si existe un $K$ tal que la sucesion $a_n < k$, es decir no sobrepasa a $k$ y queda acotada.

Las sucesiones que vimos de ejemplos se podrian decir que estan acotadas, $a_n = (-1)^n$ y $a_n = 1/n$, que las dos nunca van a ser **mas grandes que 1**


## Limites

#### Definicion

Decimos que tiene limite finito $L in RR$ si $forall epsilon > 0$, $exists n_0 in NN$ tal que $a_n in E(L,epsilon)$, $forall n gt.eq n_0$

#### Definicion limite infinito

Decimos que $ lim_(n arrow infinity) a_n = +infinity$ si $forall k > 0$, $exists n_0 in NN$ tal que $a_n > k$, $forall n gt.eq n_0$

#### Definicion monotona creciente

Decimos que $a_n$ es monotona creciente/decreciente si $a_(n+1) gt.eq a_n$/$a_(n+1) lt.eq a_n$, decimos que la monotonia es **estricta** si la definicion se cumple solo con $>$ o $<$.

Si es monotona es muy probable que tenga un limite ya sea finito o infinito. Por el simple hecho que no oscila como lo hacia $a_n = (-1)^n$entre $1$ y $-1$.

#### Teorema

1. Si es monotona creciente pueden pasar dos cosas, primero que todo es **acotada la sucesion**, asi que vamos a tener un **limite finito**, y si **no es acotad** vamos a tener un **limite infinito**.

2. Si la sucesion tiene **limite finito**, es **acotada**.

3. Si $lim a_n = plus.minus infinity$ **no es acotada**

4. Si la sucesion es acotada, puede **tener limite finito o oscilar**.

5. Si existe el limite en la sucesion es **unico**.

#### Propiedades:

Imaginemos que tenemos 

$$
lim_(n arrow infinity) a_n = A; space "y" lim_(n arrow infinity) b_n = B
$$

1. $lim(a_n + b_n) = A + B$

2. $lim(a_n dot b_n) = A dot B$

3. Si $B eq.not 0$ entonces, $lim a_n/b_n = A/B$

4. Tenemos $K in RR$ y un limite 

$$
lim_(n arrow +infinity) k a_n = k lim_(n arrow +infinity) a_n = k A
$$

5. $ a_n lt.eq b_n$ y las dos tienen **limite** enotonces $lim a_n lt.eq lim b_n$

### Definicion de equivalencia

Decimos que dos sucesiones $a_n$ y $b_n$ son **equivalentes** $(a_n ~ b_n)$ si 

$$
lim_(n arrow +infinity) a_n/b_n = 1
$$

#### Ejemplos:

1. $a_n = 3 n^2 - 5n + 8 space "y" space b_n = 3n^2$

$$
lim a_n/b_n = lim (3n^2-5n+8)/3n^2 = lim (3n^2)/(3n^2) - lim (5n)/(3n^2) + lim 8/(3n^2)
$$

### Definicion de Par de Sucesiones Monotonas Convergentes

Decimos que $a_n$ y $b_n$ forman un Par de Sucesiones Monotonas Convergentes (PSMC) si: 

1. $a_n lt.eq b_n space forall n in NN$

2. $a_n$ es creciente y $b_n$ decreciente

3. $forall epsilon > 0$, $exists m in NN$ tal que $|a_m - b_m| < epsilon$






