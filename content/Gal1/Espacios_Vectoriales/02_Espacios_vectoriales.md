---
title: 2-Espacios vectoriales
---

Para definir un espacio vectorial nesecitamos un cuerpo $KK$ y un conjunto $V$ que tenga las operaciones de suma y multiplicacion por escalar por ejemplo $(V,KK,+,dot)$.

$$
+: V times V arrow V = v_1 + v_2 space space space
dot: KK times V arrow V = lambda dot v_1
$$

## Propiedades

El espacio vectorial al estar conformado por un **cuerpo** comparte las propiedades ya mencionadas [aca](http://localhost:8080/Gal1/Espacios_Vectoriales/Introduccion_espacios_vectoriales#cuerpos), a **excepcion** de la existencia del opuesto multiplicativo que vendria a ser $1/a$, la **Conmutatividad** del producto tampoco se encuentra.
 
> [!note]- Aclaracion
> Cuando nos referimos a espacios vectoriales, el **0** va dirigido al **0** del **espacio vectorial**, por ejemplo no es lo mismo el **0** de una matriz al de un polinomio.

Esto nos deja:


- La suma y multiplicacion de 2 **elementos** que $in KK$ tiene que dar un elemento que $in KK$.

- La suma es **conmutativa** $arrow.r.double.long a+b = b+a$.

- La suma y multiplicacion son **asociativas** $arrow.r.double.long (a+b)+c = (b+c)+a$.

- La suma y multiplicacion son **distributivas** $arrow.r.double.long$ $(a+b)dot c = a c + b c$.

- Existencia del **neutro** multiplicativo y aditivo, en el caso de la multiplicacion **1** y de la suma **0**.

- Existencia del **inverso** aditivo $-a$.

> [!tip]- A mencionar 
> A los elementos de un **E.V** se le llaman **vectores**.

## Ejemplos de espacios vectoriales

1. El espacio vectorial de las matrices $m times n$ a este espacio lo denotamos como $V = (#strong[Mat]$$(RR)_(n times m), RR, +, dot)$. 

2. El espacio vectorial de los todos los polinomios con coeficiente menor o igual a **n** $V = (RR_n [x], RR, +, dot)$ donde **n** no puede ser negativo.
$$
 RR_n [x] = {a_0 + a_1 x + a_2 x^2 + dot dot dot + a_n x^n}
$$

> [!faq]-  Tip
> Mas adelante van a aparecer los subespacios vectoriales y vamos a tener que usar condiciones como $ p(x) = 0 $ esto significa que todas las funciones que "entren" ahi van a tener que cumplir que sea 0. La funcion en este caso puede perfectamente ser un polinomio

3. El espacio vectorial de las n-uplas, este puede ser representado como $V = (RR^n, RR, + , dot)$  

$$
RR^n = {(x_1, x_2, x_3, dot dot dot, x_n)}
$$
$$
$$
$$
RR^3 = {(x_1, x_2, x_3)}
$$

## Ejemplos de NO espacios vectoriales
 
1. El conjunto de los numeros naturales $NN$ no forma un espacio vectorial, directamente **no** tiene ningun **inverso aditivio** es decir $-a$.
2. El conjunto de los polinomios de grado $= 3$, tambien podria ser cualquier otro grado de polimionio.
$$
p(x) = -x^3 + x^2 + x + 1
space space
q(x) = x^3 + x^2 + x + 1
$$
$$
$$
$$
p(x) + q(x) = x^2 + x + 1
$$

que ya deja de pertenecer al E.V
