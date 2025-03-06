---
title: 9-Sumas directas
---

Bueno imaginemos que tenemos dos subespacios $S_1$ y $S_2$ que pertenecen al **E.V** $V$, bueno ya teniamos la **conocida suma de subespacios** $U + W$.

Pero ahora nos interesa aprender una forma de suma llamada **suma directa**. La cual escribiriamos asi $U plus.circle W$, y esta nos da el conjunto de todos los vectores que se pueden escribir de forma **UNICA** como la suma de un vector de $U$ y un vector de $W$.

Por ejemplo los vectores que pertenecen a este conjunto **no se pueden generar sumando un vector de** $U$ **con otro vector de** $U$, y lo mismo con $W$, solo los vectores que se pueden **generar con la suma entre dos vectores de** $U$ y $W$.

### Dato importante

Si hacemos $V = U + W$, entonces $V = U plus.circle W$ **solo si** $U sect W = 0$

### Otro dato importante

Si $V = U plus.circle W$ y $B_1$, $B_2$ son **bases** de $U$ y $W$

Entonces tenemos que $B = B_1 union B_2$ es una **base** de $V$.

Tambien considerando que $V$ sea un espacio de **dimension finita** entonces $ "dim" V = "dim" U+"dim" W$

## Ejercicios Parcial

### 1)

![Sej1](2025-02-10_04-04.png)

Bueno, primero que todo intentamos obtener un polinimio generico que pertenezca a $S_1$

Para eso podemos aplicarle las condiciones:

$$
p(1) = a x^3 + b x^2 + c x + d = 0
$$

Para que esto sea **0** con $x = 1$ entonces $a + b + c + d = 0$, la otra condicion que podemos sacar es:

$$
p(0) = a x^3 + b x^2 + c x + d arrow.r.double.long d = 0
$$

Resumiendo $d$ tiene que ser **0** asi que la condicion del subespacio queda asi $a + b + c = 0$, pasando esto a polinomio general se ve asi.

$$
a x^3 + b x^2 + c x = 0
$$

Nos damos cuenta que la base de $S_2$ es en dos terminos por lo tanto vamos a querer achicarlo tambien para conseguir la base.
Asi que ponemos a $c$ como valor de $a$ y $b$ asi:

$$
c = -a - b
$$
$$
$$
$$
a x^3 + b x^2 + (-a -b)x = 0
$$

Por lo tanto la base quedaria asi.

$$
a(x^3-x) + b(x^2-x)
$$

Igualamos las bases:

$$
a(x^3-x) + b(x^2-x) = lambda(x^3 - x^2) + alpha(x+1)
$$

Y ahora aplicamos las mismas condiciones a la base de $S_2$ para ver si existe algun vector que cumpla las condiciones de $S_1$ y de $S_2$ a la vez.

$alpha$ al ser termino independiente, ya que $p(0) =0$ tiene que ser $0$. Por lo tanto solo nos queda $lambda$.

En resumen:

$$
lambda(x^3 - x^2) + 0(x+1)
$$

$S_1 sect S_2 = {x^3 - x^2}$

**Ese vector es el unico que cumple con $S_1$ y $S_2$**

### 2)

![Sej2](2025-02-10_23-24.png)

Primero que todo nos fijamos si el conjunto de $S_1$ es linealmente independiente, para saber si es base del mismo o tenemos que sacar algun vector.

$$
lambda mat(1,0;0,1) + alpha mat(1,1;1,1)
$$

Si hacemos un sistema nos va a dar que $alpha = 0; lambda =0$ y que genera un **espacio de dimension 2**.

Ahora lo mismo con $S_2$.

$$
mat(a,a;b,b) arrow.r.double.long a mat(1,1;0,0) + b mat(0,0;1,1)
$$

Y aca tambien queda $a = 0; b=0; por lo tanto es **linealmente independiente** y es de **dimension 2**

O sea que **las dos son bases se su subespacio**.

>[!note] Buscar en deepseek la parte b 






