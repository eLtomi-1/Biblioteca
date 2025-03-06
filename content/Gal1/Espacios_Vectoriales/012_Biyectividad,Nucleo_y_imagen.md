---
title: 12-Biyectividad, Nucleo e imagen de una transformacion lineal.
---
## Inyectividad, Sobreyectividad y Biyectividad

Las tranformaciones lineales pueden ser **inyectivas, sobreyectivas y biyectivas**

- **Inyectiva** - imaginemos que tenemos $v,v prime in V$, es **inyectiva si** $T(v) eq.not T(v prime)$ en todos los casos, es decir siempre da vectores diferentes.

- **Sobreyectiva** - es solo si teniendo en el espacio de entrada siempre va a tener un vector en la salida es decir. $v in V; w in W$ siempre pasa esto $T(v) = w$

- **Biyectiva** - esto se cumple si se cumplen las dos anteriores y se dice que es un **Isomorfismo**

## Nucleo e imagen

Considerando $v in V; w in W$ y $T:V arrow.r W$.

- **Nucleo (kernel)** de una transformacion lineal representado como $"ker"(T)$ como el **conjunto de vectores** que generan $T(v) = 0_v$

- **Imagen (rango)** de una transformacion lineal representado como $"Im"(T)$ como el conjunto de **todos los vectores que se pueden generar** usando la transformacion $T$.

>[!important] 
> El **nucleo** de $T$ es un **subespacio** de $V$
> 
> La **imagen** de $T$ es un **subespacio** de $W$

## Datos IMPORTANTES

Como saber si es **inyectiva**:

1. $"ker"(T) = {0v}$

2. Si tenemos un conjunto **linealmente independiente** llamado $L$, si hacemos $T(L)$, nos va a dar un conjunto **linealmente independiente**

3. $"dim"(V) < "dim"(W)$

Como saber si es **sobreyectiva**:

1. $"Im"(T) = W$

2. Si tenemos un cojunto generador $G$ y usamos la funcion $T(G)$ tambien se cumple que sigue siendo generador pero en $W$

3. $"dim"(V) > "dim"(W)$

Si tenemos un isomorfismo $T$ y $C={v_1,v_2, dot dot dot, v_n}$ un conjunto de elementos en $V$

1. $T^(-1) : W arrow.r V$ sigue siendo un isomorfismo.
2. $C$ es (**linealmente independiente, una base o un generador**) si $T(C) = {T(v_1), T(v_2), dot dot dot, T(v_n)}$ es (**linealmente independiente, una base o un generador**).
3. $"dim"(V) = "dim"(W)$
