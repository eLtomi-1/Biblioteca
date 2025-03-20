---
title: 2- Ecuaciones Diferenciales
---

Ecuaciones diferenciales se refiere a las ecuaciones donde aparecen las derivadas, mas que nada **"diferenciales"** se refiere a sus derivadas.

Primero que todo generalmente siempre resolvemos este tipo de ecuaciones:

$$

x in RR space x^2 = 2 ,

$$
$$
$$
$$

z in CC space z^8 = 2 

$$

Ahora van a ser asi:

$$ 
f prime (x) = f(x) 
$$

Una solucion de esta ecuacion puede ser $f(x) = e^x$ ya que la derivada de $f(x)$ es lo mismo que $f(x)$

### Notacion

La notacion de $x(t)$ seria simplemente $x$ y $x prime (x)$ va a pasar a ser $x prime$

## Metodos de resolucion de Ecuaciones diferenciales de variables separables

Estas de representan asi:

$$
x prime (x) = F(x(t)) dot H(t)
$$

Aca tenemos ejemplos de como deberian de ser:

1. $x prime (x) = x(t) dot 1$, Este **si es valido**
2. $x prime (x) = x(t) dot z^2$, Este **si es valido**
3. $x prime (x) = x(t) + t$, Este **no es valido**

#### Ejemplo 1:

$$
x prime (t) = x(t) dot t arrow.r.double.long (x prime (x))/x(t) = t 
$$

Entonces integremos.

$$
integral (x prime (x))/x(t) = integral t
$$

Aca tenemos nada mas que hacer un cambio de variable en **la integral izquierda**.  Y la parte derecha se integra sola.

$$
integral 1/u d
u = t^2/2 arrow.r.double.long ln(u) = t^2/2 arrow.r.double.long x(t) = e^(t^2/2)
$$

Esto viene a ser el metodo, ya que siempre vamos a poder hacer el cambio de variable porque vamos a tener de un lado la derivada de la funcion $x$ y del otro lado la funcion $x$.

#### Ejemplo 2:

$$
x prime (t) = (1 + x^2(t)) dot 3t^2 arrow.r.double.long (x prime (t))/(1 + x^2(t)) = 3t^2
$$

Ahora hacemos lo mismo e integramos:

$$
integral (x prime (t))/(1 + x^2(t)) = integral 3t^2 arrow.r.double.long integral 1/(1 + u^2) d u = integral 3 t^3
$$

Resolvemos:

$$
arctan(x(t)) = t^3
$$

## Ecuaciones diferenciales lineales de 1er orden

Ahora vamos a ver como calcular este tipo de ecuaciones diferenciales

$$
x prime (t) + a(t) dot x(t) = b(t)
$$

Vamos a tener 2 tipos de estas ecuaciones:

> [!note]
> **Teorema**: La solucion general de **NH** se obtiene como la suma de la **solucion general** de **H** mas una solucion particular de **NH**.

- **H** (Ecuacion homogenea) $x prime (t) + a(t) dot x(t) = 0 $, que ya sabemos como solucionar esta porque fue el metodo que mostramos antes. El espacio de las soluciones de este tipo de ecuaciones genera un **espacio vectorial** de $"dim"(V) = 1$

- **NH** (Ecuacion no homogenea) $ x prime (t) + a(t) dot x(t) = b(t) $, y la solucion de esta se representa asi $x_"NH" (t) = x_"H" (t) dot x_"P" (t) = 0$, siendo $x_"NH" (t)$ la **solucion general de NH**, $x_"H" (t)$ la **solucion general de H** y $x_"P" (t)$ una **solucion  particular de NH**


#### Ejemplo

Primero que todo tenemos esta ecuacion $x prime (t) - cos(t) dot x(t) = cos(t)$ 

Tenemos que hayar la solucion general de la **homogenea**, que la ecuacion a resolver seria $x prime - cos(t) dot x = 0$

$$
x prime = cos(t) dot x arrow.r.double.long (x prime)/x = cos(t)
$$

Esto lo pasamos para integrar y nos va a quedar asi $integral (x prime)/x = cos(t)$

$$
integral 1/u dot d u = integral cos(t)
$$
$$
$$
$$
 ln(|x(t)|) = sin(t) arrow.r.double.long x(t) = k dot e^sin(t) 
$$

Por lo tanto la solucion general de la homogenea es $k dot e^sin(t)$

Ahora queremos hayar una solucion particular de la no homogenea:

Vamos a usar el **metodo de variacion de constantes**:


## Ecuaciones diferenciales lineales de 2do orden

Bueno para empezar estas funcionan bastante parecido a las de primer orden y las representamos asi.

$$
y prime prime (x)  + a y prime (x) + b y (x) = h(x)
$$

Como ya dijimos hay dos tipos de esta, la **homogenea* y la **no homogenea**.

$$
y prime prime (x)  + a y prime (x) + b y (x) = 0
$$
$$
$$
$$
y prime prime (x)  + a y prime (x) + b y (x) = h(x)
$$

El espacio posible de soluciones de **H** es de $"dim"(V) = 2$

Y de vuelta la **solucion** general de la **NH** es la solucion general de **H** y una solucion especifica de la **NH**.

Para **resolver la homogenea** vamos a buscar soluciones de la forma $y(x) = e^(lambda x)$

Podemos decir que este es el valor de $y$ ya que siempre como resultado $a y prime (x) + b y (x)$ nos va a dar una exponencial en $e$.

Por lo tanto $y prime prime (x)= e^(lambda x) lambda^2$ y $a y prime (x) = e^(lambda x) lambda$.

Si **sustituimos** nos queda asi:

$$
lambda^2 e^(lambda x) + a lambda e^(lambda x) + b e^(lambda x) = 0
$$

Sacamos factor comun:

$$
e^(lambda x) (lambda^2 + a lambda + b) = 0
$$

Y si nos damos cuenta $e^(lambda x)$ no puede ser **0** ya que es una **exponencial**, por lo tanto solo $(lambda^2 + a lambda + b)$ puede ser **0** y si esto se cumple significa que el valor de $lambda$ es raiz.

Por lo tanto le podemos hacer **bhaskara**, esto se va a dividir en **3 posibles casos**:

- El primero nos van a generar dos raices distintas ${e^(lambda x), e^(lambda_2 x)}$ y el resultado de la homogenea quedaria asi $y_"H" = alpha e^(lambda x) + beta e^(lambda_2 x)$ 

- El segundo es que nos genera dos raices **iguales** por lo tanto nos caga porque deberiamos de tener un espacio de **dimension 2** y con esto solo generamos **uno**. Aca como solucion tendriamos que $y_"H" = alpha e^(lambda x) + beta x e^(lambda_2 x)$

- El tercero es que las raices son **raices complejas**, estas las podemos representar asi $lambda_1 = a + b i$ y su **conjugado** $lambda_1 = a - b i$

#### Ejemplos

1. $y prime prime - 5 y prime + 6 y = 0$

Esto lo podemos pasar a $e^(lambda x) lambda^2 - 5 e^(lambda x) lambda + 6 e^(lambda x)$

Y luego lo factorizamos $e^(lambda x) (lambda^2 - 5 lambda + 6) $

Ahora hacemos bhaskara al segundo termino que es el que depende para que sea **0** y nos da $lambda = 3; lambda_2 = 2$



