---
title: Practico 3
---

Sucesiones

**1)** 
![PC2](2025-03-29_02-14.png)

**a)** Primero que todo queremos ver si tiene un **limite** y a donde tiende.

$$
lim_(n arrow plus infinity) 1 + 1/n = 1
$$

Nos damos cuenta que si tiene un limite hacia $1$ por lo tanto es convergente en uno.

Ahora queremos saber si esta acotada, por lo tanto queremos saber el maximo valor que puede obtener esta sucesion, ya sea **infinito** o un numero $k$, si nos damos cuenta.

La sucesion avanza asi $a_1 = 1+1; space a_2 = 1 + 1/2; space a_3 = 1 + 1/3$, como podemos ver lo unico que va haciendo es a partir del **2** ir cada vez mas cerca del uno.

Asi que nos queda acotada asi $1 < a_n lt.eq 2$ ya que el uno no lo toca nunca.

Y ahora queremos saber si es **monotona**, como podemos ver decrece hacia el uno asi que tenemos que probar que es **monotona decreciente**.

$$
a_(n+1) < a_n arrow.r.l.double 1+1/(1+n) < 1+1/n
$$
$$
$$
$$
a_(n+1) < a_n arrow.r.l.double 1/(1+1/(1+n)) > 1/(1+1/n)
$$

El inverso del inverso en este caso es igual a $n+1$ o $n$

$$
a_(n+1) < a_n arrow.r.l.double n+1 > n
$$

Nos queda que $n+1 > n$, que esta sucesion mientras mayor es el $n$ mas chico es el resultado que devuelve por lo tanto se cumple $a_(n+1) < a_n$ haciendola **monotona decreciente**.

**b)** En esta primero que todo podemos hacerle el limite para ver si esta acotada

$$
lim_(n arrow plus infinity) 1 + (-1)^n/n = 1
$$

Es convergente porque tiene un limte en **1** por lo tanto converge en ese numero, tambien nos damos cuenta que no es monotona porque no siempre $n+1 > n$ ni $n+1 < n$

Queremos ver en que numeros esta acotada, sabemos que el 1 seguro y el 0 que el uno nunca lo toca, y el cero es el numero mas chico que alcanza. Por lo tanto $1 > a_n gt.eq 0$

**c)** Vamos a hacerle el limite:

$$
lim_(n arrow plus infinity) n + 1/n = n = plus infinity
$$

Rapidamente nos damos cuenta de que no es acotada porque tiene un **limite infinito**, tambien nos damos cuenta si calculamos los valores que siempre el resultado va a ser $n$ sumado de una fraccion muy chica, por lo que hace que sea **monotona decreciente**, (cosa que aun no se probar).

Tampoco es **convergente** ya que el limite esta tendiendo a un valor **infinito** y no **finito**. Cuando no es convergente es **divergente**.

**d)** Ahora que aprendi a como probar que sea monotona creciente por absurdo vamos a ver primero de todo si es acotada:

$$
lim_(n arrow plus infinity) n/(sqrt(n^2+1)) = 1
$$

Es acotada en a_n < 1, y converge en $1$, ahora tenemos que ver si es monotona creciente.

$$  
a_(n+1) > a_n; arrow.r.double.long n+1/(sqrt((n+1)^2+1)) > n/(sqrt(n^2+1)) 
$$

Si hacemos las cuentas nos va a dar que $2n+1 > 0$ cosa que es verdad porque $n$ siempre es positivo. La resolucion esta [aca](https://youtu.be/BLr7d7nJnIk?si=1FBczrVefkets1mf&t=2656)


