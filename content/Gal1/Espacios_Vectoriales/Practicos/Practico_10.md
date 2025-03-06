---
title: Practico 10
---

Transformaciones lineales

### 2)

![Tlej2](2025-02-18_01-22.png) 

**a)** Aca lo que tenemos que hacer es haya la transformacion para todo polinomio $p$.

Si nos damos cuenta ya nos dieron una base canonica esto ayuda muchisimo.

$$
lambda (1,0) + alpha (1,1) + beta (0,0) 
$$

Como tenemos la base canonica solo modificamos los valores por lo de la transformacion y sumamos. 

$$
T(p) = (lambda + alpha, alpha)
$$

Esta es la original.

**b)** Primero que todo para responder la pregunta si solo hay una, es si porque es una base y las bases en el otro lado son unicas.

Hayemos $T(3,2,1)$

$$
(3,2,1) = lambda (1,0,0) + alpha (1,1,0) + beta (1,1,1)
$$

Si hacemos la matriz queda $lambda = 1; alpha = 1; beta = 1$ asi que la transformacion queda asi:

$$
T(3,2,1) = (2,1,0) + (-1,2,3) + (0,0,1) = (1,3,4)
$$

**c)** Primero queremos saber si existe la transformacion $T(3+2x+x^2) = (2,1)$

$$
3+2x+x^2 =  lambda (1) + alpha (x+1) + beta (1+x+x^2)
$$
$$
$$
$$
3+2x+x^2 =  (lambda + alpha + beta) + (alpha + beta) x + (beta) x^2
$$

Ahora con esto podemos averiguar las coordenadas, que son $lambda =1; alpha =1; beta = 1$.

$$
T(3+2x+x^2) =  (1,0) + (1,1) + (0,0) = (2,1)
$$

Por lo tanto **si existe esa transformacion** ahora tenemos que hayar la **transformacion general**.

Tenemos que hacer lo mismo pero con el **vector canonico**

$$
a x^2 + b x + c =  (lambda + alpha + beta) + (alpha + beta) x + (beta) x^2
$$

Nos da las coordendas que son $lambda = c-b; alpha = b-a; beta = a$

Suplantamos

$$
a x^2 + b x + c =  (c-b) (1,0) +(b-a)(1,1) + a (0,0)
$$

Si sumamos todo nos da que el generico es $T(a x^2 + b x + c) =k(c-a, b-a)$








