---
title: 2- Recursion
---

Bueno como antes la induccion **servia para probar propiedades**, la recursion sirve parar definir funciones sobre los elementos del conjunto

$NN subset.eq RR$ definido inductivamente por:

1. $0 in NN$
2. Si $n in NN$, entonces $S(n) in NN$

### ERP (Esquema de recursion primitiva) para $NN$

Imaginemos que tenemos que definir la funcion **factorial** en base a los naturales.

La podemos definir asi $"fact"(0) = 1$, primero el elemento base, ahora definimos como funciona para los demas o sea las sucesiones de $n$, $"fact"(S(n)) = "fact"(n) dot S(n)$

Es claro que es una recursion.

#### Ejemplos 

Tenemos que hacer la funcion que mida el **largo** de un **string** $Sigma^*$ en este caso $"Largo"()$:

$$
"Largo"(epsilon) = 0
$$
$$
$$
$$
"Largo"(x w) = "Largo"(w) + 1
$$

Tambien tenemos la funcion $"Espejo"()$

$$
"Espejo"(epsilon) = epsilon
$$
$$
$$
$$
"Espejo"(x w) = x "Espejo"(w) x
$$

Si hacemos la recursion pasando "abc", $"Largo"()$ nos va a devolver **3** y $"Espejo"()$ nos devuelve "abccba".

Cada vez que queremos definir una funcion tiene que cumplir con **tres** cosas:

1. Exhaustividad, es decir todo elemento del dominio tiene que computar algun valor.
2. No superposicion, ningun elemento del dominio puede computar a mas de un valor.
3. Terminacion, las llamadas recursivas usan elementos menores.

### Resumen 

1. No se aplica **ERP** si la definicion inductiva del conjunto no es **libre**, o sea que no todos los elementos se generan de manera unica.

2. Si la definicion no es libre, hay que probar que los casos repetidos dan el mismo resultado.

3. Si se usa **ERP**, hay que probar **exhaustividad**, no superposicion y terminacion.


