---
title: 1- Numeros Complejos
---

Bueno primero de todo que es un numero complejo, bueno un **numero complejo** es un **par ordenado** (un par ordenado son unas coordenadas que si las invertimos no son iguales por ejemplo $(x,y)$ o sea que el orden importa)

Le llamamos **parte real** a $x$ (primer elemento), e imaginaria a $y$ (segundo elemento)

Imaginemos que $(a,b)$ y $(c,d)$.

1. Decimos que $(a,b) = (c,d)$ si $a = c$ y $b=d$.
2. Decimos que $(a,b) + (c,d) = (a+c,b+d)$ 
3. Decimos que $(a,b) dot (c,d) = (a c - b d, a d + b c)$

Un dato muy importante es que $i^2 = -1$.

>[!note]-
> Si nosotros hacemos $(0,1) dot (0,1) = (0 - 1, 0 + 0) = (-1,0)$

>[!important]
> $i = (0,1)$
> 
> Ya que $(a,b) = (a,0) + (0,b) = a(1,0) + b(0,1) = a dot 1 + b dot i$.
> 
> Que a su vez esta notacion se llama **notacion binomica**.

### Notacion Binomica y Polar

La **binomica** se puede expresar de la siguiente manera $z = x + i y$

La **polar** se expresa asi donde $r=sqrt(x^2 + y^2)$ quedaria asi $z = r e^i arctan(y/x)$

 

### Modulo de un complejo

El modulo es decir el largo o el espacio que ocupa de un numero complejo es, $|z| = sqrt(x^2 + y^2)$

Tambien esta su **argumento** que viene a ser el angulo que esta entre $|z|$ y el eje $x$.

![Cdimg](2025-03-06_16-45.png)

### Argumento de un complejo

El argumento se puede calcular haciendo el $arctan(y/x)$

### Valores de a y b

Mas que nada para pasar de una **notacion polar** a una **binomica**, definimos **a** y **b**.

$ a = r cos(alpha) $

$ b = r sin(alpha) $

### Conjugado del numero complejo

$z^- = x - y i$

Cambiamos de signo la parte que esta multplicando a $i$.

### Propiedades de los numeros complejos.

1. $|z| gt.eq 0$
2. $|z| = 0$ si $z = 0$
3. $|"Re"(z)| lt.eq |z|$; $|"Im"(z)| lt.eq |z|$
4. $|z dot w| = |z| dot |w|$ y lo mismo con la **division**
5. $|z + w| lt.eq |z| + |w|$

#### Formula para averiguar las raices enesimas 

$$
z_k = root(n, r) dot e^i((alpha + 2 pi k)/n)
$$

### Exponencial compleja

$$
e^z = e^x cos(y) + i sin(y)
$$

El modulo de $|e^z| = e^x$ y el argumento es de $e^z$ es $y$.
