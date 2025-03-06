---
title: 3-Subespacios vectoriales
---

Ya sabiendo que son los espacios vectoriales ahora tenemos los **Subespacios vectoriales** que ahora seran **S.V**.

Supongamos que tenemos el **E.V**, $V = (V,KK,+,dot)$ *(El generico)*

Bueno un **S.V** de $V$ es un subconjunto de $V$, que tambien copia las operaciones de suma y multiplicacion de $V$, al subconjunto le llamaremos $W$.

## Como sabemos si es un Subespacio

Para verificar si es un **S.V** tiene que cumplir las mismas condiciones para que un **E.V** mencionadas [aca](http://localhost:8080/Gal1/Espacios_Vectoriales/Espacios_vectoriales#propiedades), sin necesidad de verificar las propiedades de conmutatividad, distributividad y asociatividad.

### Definicion

Suponiendo que tenemos un $KK$-espacio vectorial llamado $V$ y un subconjunto $in V$ llamado $W$. Podriamos decir que $W$ es un subespacio de $V$ si cumple:

- Es cerrado bajo la **suma** y la **multiplicacion**.
- Contiene al **0**, es decir el vector nulo de $V$.

> [!note]- Dato
> Los **S.V** no pueden ser conjuntos vacios.

## Ejemplos de Subespacios

> [!note]- Definicion
> Un subespacio trivial es cuando esta solo compuesto por ${0}$ o es $V$ entero.

- El subespacio ortogonal $< u, v > = 0$ que pertenece al espacio $RR^2$, cumple con la suma y la multiplicacion ademas de contener el **0**.
- Subespacios de $RR [x]$, cada $RR_n[x]$ es un subespacio distinto de $RR [x]$.

- Subespacios no triviales de $RR^3$, en realidad esto significa que no puede ser ${0}$, por lo tanto justo en este **E.V** hay dos subespacios asi, el subespacio de las rectas y el de los planos.

- Otro ejemplo seria el subespacio de las matrices simetricas $#strong[Mat]$$(RR)_(n times n)$. 

## Ejemplos de NO Subespacios

- Consideremos el ejemplo en el cual $W = {A in #strong[Mat]$$(RR)_(2 times 2): A^2 = A}$, en este **S.V** unos de los ejemplos es la matriz.

$$
mat(1,1;1,1)^2 = mat(1,1;1,1)
arrow.r.double.long
mat(1,1;1,1) + mat(1,1;1,1) = mat(2,2;2,2)
$$

> [!warning] La posta
> La suma de dos matrices del mismo subespacio no quedo cerrado en el espacio, por lo tanto no es un subespacio.

- Otro que tampoco cumple es $W = {A in #strong[Mat]$$(RR)_(2 times 2): det(A) = 0}$, 

$$
mat(1,0;0,0) + mat(0,0;0,1) = mat(1,0;0,1)
$$
$$
$$
$$
$$
$$
(det(A) = 0) + (det(B) = 0) = (det(A+B) eq.not 0)
$$
