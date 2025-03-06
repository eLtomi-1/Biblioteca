---
title: 6-Dependencia e independencia lineal
---

Imaginemos que tenemos el **E.V** llamado $V$, tenemos el conjunto no vacio $S = {v_1, v_2, dot dot dot, v_n}$

Bueno el conjunto $S$ serie **linealmente dependiente**, si hay escalares $lambda_1, lambda_2, dot dot dot, lambda_n$ **sin ser todos iguales a 0** tales que:

$$
lambda_1 v_1 + dot dot dot + lambda_n v_n = #strong[0]
$$

Si no existen esos escalares decimos que el conjunto $S$ es **linealmente independiente** si cumple lo siguiente.

$$
lambda_1 v_1 + dot dot dot + lambda_n v_n = #strong[0], space lambda_i = 0
$$

O sea que si todos los escalares son 0, es **linealmente independiente**.

> [!note]- Dato
> Un conjunto que no es linealmente dependiente se dice linealmente independiente.

## Primer ejemplo

Consideramos que tenemos el **E.V**, $V = RR^2 [x]$ y el conjunto $S = {1+x,2-x^2, 3+x-2x^2}$

Si igualamos el **0** como combinacion lineal de los elementos de $S$

$$
lambda(1+x) + alpha(2-x^2) + beta(3+x-2x^2) = 0
$$

Vamos a ordenar los terminos para mostrar como deberia de quedar **siempre** en estos casos.

Primero **desarrolamos todas las cuentas**:

$$
lambda + 2 alpha + 3 beta + lambda x + beta x - alpha x^2 - 2 beta x^2
$$

Luego las ordenamos y listo

$$
(lambda + 2 alpha + 3 beta) + (lambda + beta) x + (- alpha - 2 beta) x^2
$$

Ahi quedo, ahora para que todo esto se cumpla para todos los $x$ cada termino tiene que ser **0** asi que armamos y resolvemos este sistema.

$$
 cases(
    lambda + 2 alpha + 3 beta = 0 \
    lambda + beta = 0\
    - alpha - 2 beta= 0 
)
$$

En este caso se puede **resolver como matriz** o por intuicion, ya que concordamos que la **unica solucion** del sistema es que $lambda, alpha, beta$ sea igual a **0**.

Asi que conlcluimos que es **linealmente independiente**.

## Segundo ejemplo

Supongamos que tenemos el **E.V**, $V = #strong[Mat]$ $(RR)_(2 times 2)$ y el conjunto de matrices $S = {mat(1,0;0,0),mat(0,1;0,0),mat(0,0;1,0),mat(0,0;0,1)}$ 

Primero vamos a ponerlo como una combinacion lineal:

$$
lambda mat(1,0;0,0) + alpha mat(0,1;0,0) + beta mat(0,0;1,0) + d mat(0,0;0,1) = mat(0,0;0,0)
$$

Justo en este caso es tan facil como hacer las cuentas

$$
mat(lambda, alpha; beta, d) = mat(0,0;0,0)
$$

Lo que significa que $lambda = alpha = beta = d = 0$

## Dato importante

Suponiendo que tenemos un **E.V** llamado $V$ y un conjunto llamado $S = {v_1, v_2, dot dot dot, v_n}$ que pertenecen a $V$ con $n gt.eq 2$.
 
Entonces $S$ es **linealmente dependiente** si unos de los vectores $v_i$ es combinacion lineal de los demas vectores en $S$.

### Ejemplo

Imaginemos que tenemos el **E.V**, $V = RR^3$

Si usamos el **dato importante** recien mencionado para el caso $n = 2$, podemos concluir que $v_1,v_2 in RR^3$ son linealmente dependientes si y solo si **son colineales**, es decir **pertenecen a la misma recta**

## Otro dato importante

De vuelta imaginemos que tenemos un **E.V**, $V$ y un conjunto finito de vectores $S$

1. Si $S$ es linealmente independiente y $S_1$ es un subconjunto no vacio de $S$, entonces $S_1$ tambien es **linealmente independiente**.
2. Si $S_1$ es un subconjunto no vacio de $S$ que es linealmente dependiente, entonces $S$ tambien es **linealmente dependiente**


## Ultimo dato importante

Cuando vos le haces **el determinante** a una matriz $A$, por ejemplo $|A| = 0$, y el determinante da **0**, los vectores que la componen son **linealmente dependientes**

Si vos le haces **el determinante** y da $|A| eq.not 0$ entonces los vectores que componen a $A$ son **linealmente independientes**.



