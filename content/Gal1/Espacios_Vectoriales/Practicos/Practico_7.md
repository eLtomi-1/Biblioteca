---
title: Practico 7
---

Espacios y subesapacios vectoriales.

> [!note] Aclaracion
> **R:** 
> Significa **R**espuesta


### 1) 

![Pej1](2025-01-23_02-28.png)

Como dice la consigna, tenemos que investigar si cada uno de los ejemplos son **E.V** en base a las operaciones de suma y producto (claramente son una verga).

**a)** Con la suma en este caso no tenemos nada raro ya que esta cerrado y tenemos el neutro. Pero luego con el **producto** tenemos el problema que **no tenemos el neutro**. Por ejemplo:

$$
lambda (x_1,y_1) = (3 lambda y_1, x_1)
$$

Si pusieramos el caso en el que $lambda = 1$ es decir el neutro multiplicativo.

$$
 (x_1,y_1) eq.not (3 y_1, x_1)
$$

Como podemos si lo multiplicamos por el neutro no queda igual cuando si deberia.

**b)** En este ejemplo sucede exactamente lo mismo que en el anterior, **no tiene neutro multiplicativo**.

$$
lambda (x_1,y_1) = (lambda x_1, 0)
$$

Si pusieramos el caso en el que $lambda = 1$ es decir el neutro multiplicativo.

$$
 (x_1,y_1) eq.not (x_1, 0)
$$

**c)** En este caso no existe el neutro de la suma y lo podemos representar asi:

$$
 (x_1,y_1) + (x_2,y_2) = (x_1 + x_2, 0)
$$

Si hicieramos un caso en el cual lo unico que hacemos es sumarle 0

$$
 0 + ((x_1,y_1) + (x_2,y_2)) eq.not 0 + (x_1 + x_2, 0)
$$

Claramente al sumarles el neutro no son iguales.

**d)** Con este ya nos imaginamos por donde viene la mano, claramente no van a ser iguales siempre si le sumamos el neutro, por lo tanto **no existe el neutro de la suma**, caso muy parecido al anterior.


**e)** En este caso ya podemos ver que **no existe el neutro del producto**, si tenemos dos valores negativos del otro lado van a ser positivos. Ademas de que el **neutro de la suma tampoco**, va a pasar lo mismo.

### 2) 

![Pej2](2025-01-23_03-23.png)

> [!note]- Nota
> En mi opinion personal, no es un espacio vectorial mismo porque nunca va a tener el $(0,0,0)$. Tocara preguntarlo o investigarlo

No es un espacio vectorial porque **no** tiene el **neutro de la suma**. Hay que hacer una comparacion como las que hicimos en el ejercicio anterior.

> [!warning] Explicacion
> Los que voy salteando son los ejercicios que pide demostrar

### 5) 

![Pej5](2025-01-23_03-58.png)

> [!note]- Dato curioso
> En las funciones reales el **0** de las mismas es cuando cumple $f(x) = 0$

**a)** Se nos presenta el subconjunto $f(x) = 0$ que si queremos pasarlo a subespacio se podria representar asi:

$$
S = {f(x), x in RR | f(x) = 0}
$$

En este caso podemos definir que tiene el **0** adentro del subespacio, ya que todas las funciones que van a estar ahi valen 0. 

Tambien esta cerrado bajo la suma ya que si sumamos $ f(x) = 0$ y $g(x) = 0$ nos daria $ g(x) + f(x) = 0$ por lo tanto **sigue perteneciendo al subespacio**.

Y en cuanto al producto **cualquier cosa multiplicadada por 0 da 0**, $lambda dot 0 = 0$

**b)** En este caso tambien podemos sacar que tiene el **0**, pero ya de por si la suma de dos funciones que tengan raiz, **no significa que la suma de estas tambien tenga una raiz**.

> [!note]- Observacion
> Para mi tampoco es cerrado bajo el producto pero no sabria como explicarlo en este caso

Por lo tanto **no es un subespacio vectorial**.

### 6)
![Pej6](2025-01-23_04-37.png)
![Pej62](2025-01-23_04-38.png)

**a) R:(Si es)** Este subespacio tiene el **0**  (vamos a usar de ejemplo las matrices $2 times 2$) ya que $ mat(0,0;0,0)^t = mat(0,0;0,0) $ por lo tanto cumple que $A^t = A$

Tambien es **cerrado bajo la suma** ya que si sumamos $ mat(1,2;2,1) + mat(2,3;3,2) = mat(3,5;5,3)$ el resultado **sigue siendo simetrico**.

Y por ultimo tambien es cerrado bajo el producto $lambda mat(1,2;2,1)$ por cualquier valor que le des a $lambda$ **siempre va a ser simetrica**

**b) R:(Si es)** Este subconjunto tiene el **0** $ mat(0,0;0,0)^t = - mat(0,0;0,0) $.

Justo este subconjunto es raro porque no termino de determinar si la suma de dos matrices antisimetricas $2 times 2$ es en realidad cerrada bajo la suma, la respuesta real es que si, asi que damos como correcto que es un subespacio.


> [!note]- Observacion
> Si esto $ mat(1,0;0,-1) $ y esto $ mat(0,1;-1,0) $ son matrices antisimetricas tenemos un problema, porque la segunda estoy seguro que es antisimetrica pero no tanto de la primera.

**c) R:(No es)** En este caso para anadir un poco de contexto vamos a definir el subespacio, ya que es invertible si el $det(A) eq.not 0$

$S ={#strong[Mat]$$(RR)_(n times n), n in NN | det(A) eq.not 0}$

Primero que nada este subconjunto no contiene al **0** ya que el $det(mat(0,0;0,0)) = 0$

Por lo tanto **no es un subespacio vectorial**.

**d) R:(No es)** Este subconjunto lo podriamos definir de la siguiente manera.

$S ={#strong[Mat]$$(RR)_(n times n), n in NN | det(A) = 0}$

Como podemos ver tiene el **0** ya que el $det(mat(0,0;0,0)) = 0)$

Pero **no esta cerrado bajo la suma** directamente vamos a agarrar dos matrices que su $det(A) = 0$

$$
mat(1,1;0,0) + mat(0,0;1,1) = mat(1,1;1,1)
$$

Que en realidad si bien estas dos su determinante vale **0** $mat(1,1;0,0)$ y $mat(0,0;1,1)$ el del resultado **no** $mat(1,1;1,1)$.

**e) R:(No es)** Esta la podemos deducir, la unica matriz que tiene rango **0** es la misma matriz **nula**, por lo tanto el **unico valor** de $k$ que lo va a contener va a ser el 0. 

Y si nos damos cuenta el valor 0 de $k$ solo tiene una matriz y es la **nula tambien** por lo tanto se convierte en un subespacio trivial que tampoco es lo que andamos buscando.

**f) R:(Si es)** Las matrices con traza 0 es decir cuando nos referimos a la suma de la diagonal, es la diagonal de **arriba a la derecha hasta abajo hacia la izquierda**kj

Por lo tanto este subconjunto **si contiene** al **0**. 

Por mas que parezca raro si la **suma de los numeros de la diagonal da 0** y le sumas otra que cumpla la misma condicion, **va a seguir dando 0** 

Si tenes dudas de la anterior hacete las cuentas y vas a ver, y bueno lo mismo con **el producto totalmente funcional**.

Asi que en conclusion **es un subespacio vectorial**.

> [!important] Importante
> Dejo los sub-ejercicios de este ejercicio hasta aca ya que **no se consideran tan importantes como los otros**.

### 7)

![Pej7](2025-01-24_01-32.png)

**a)** En realidad la primera es bastante facil, si nos damos cuenta $(a,b,c) eq.not 0$ por lo tanto la unica manera para que exista el **0** en el subespacio es que $(x,y,z)$ pueda ser $= 0$. 

Pero si $(x,y,z) = 0$ significa que **por ser producto punto** el resultado va a ser **0** ahi dandonos la condicion para que exista el **0**.

Que es que $d=0$


**b)** En este pasa exactamente lo mismo que en el **a)** pero con producto cruz/vectorial en vez de producto punto.

**c)** La respuesta es decepcionante porque es literalmente $r = 0$ si no no existiria el **0** ya que el unico vector con **norma 0** es el **vector nulo**, por lo tanto solo existe ahi.

(muy obvio) pero el problema viene cuando te dicen que "fijan $r$" cosa que interprete como que r no la podias condicionar, **mal interpretado**.

Resumiendo es un **subespacio trivial** (solo contiene a el vector nulo), que cuenta como subespacio.

### 8)

![Pej8](2025-01-24_02-06.png)
![Pej81](2025-01-24_02-19.png)
![Pej82](2025-01-24_02-19_1.png)
![Pej83](2025-01-24_02-19_2.png)


**a) 1.** No es un subespacio de $RR^3$ porque no contiene al **0**, 

$0 + 0 + 0 eq.not 2$

**2.** Mismo que antes, no entra el $(0,0,0)$

**3.** En este si entra el $(0,0,0)$ ya que directamente tiene la condicion que las **3 cordenadas sean iguales** y no tiene ningun problema con la suma y el producto.


**b) 1.** Contiene el **0**, tambien esta cerrado bajo la suma:

$$
(1, dot dot dot) + (2, dot dot dot) = (3, dot dot dot)
$$

Pero si vamos al producto y multiplicamos cualquiera de estos vectores $dot -1$:

$$
lambda = -1
$$
$$
$$
$$
lambda(1, dot dot dot) = (-1, dot dot dot)
$$

Aca ya nos damos cuenta que no cumple la condicion de $x_0 gt.eq 0$

**2.** Este **es un subespacio vectorial** ya que tiene todo, el **0**, la suma cerrada y el producto cerrado.

**3.** Este **no es un subespacio vectorial** ya que el **0** no esta incluido porque todos los valores tienen que ser $= 1$

**c) 1.** En este ejemplo esta el **0**, esta cerrado bajo la suma y el producto. **Es subespacio vectorial**
**2.** En este ejemplo esta el **0**, esta cerrado bajo la suma y el producto. **Es subespacio vectorial**

> [!note] Aclaracion
> Por mas que sea igual a la derivada no pasa nada porque el valor de esta va a ser 0.

**3.** No es un subespacio porque no esta cerrado por la suma, si nos damos cuenta perfectamente podria ser $n = 1$ y hacer:

$$
p(x)=x, space g(x)=-x
$$

Si hacemos $p(x)+g(x)$

**d) 1.** Es un subespacio, contiene el **0** y en realidad como al fin y al cabo no sumamos las funciones, sumamos los valores que nos dan las funciones y no hay nada que afecte a estas, lo mismo con el producto, estos quedan cerrados.

**2.** No es un subespacio porque si bien contiene el **0** no sucede con el anterior, en este caso si bien el $f(x^2)$ no molesta el $f(x)^2$ si molesta porque altera el valor de la funcion. 

> [!warning] Lo que yo entendi
> En realidad las explicaciones de las dos anteriores no me parecen validas asi que toca gpt. 

**3.** Es un subespacio vectorial ya que el **0** es par, la suma entre numero par y otro numero par da **como resultado un numero par** y si multiplicamos un numero par por un escalar nos va a dar como resultado un numero par.


### 11)

![Pej11](2025-01-24_04-53.png)

**a)** El **0** entra en las categorias de las funciones continuas, (esto no lo sabia) pero si **sumamos dos funciones continuas nos da en efecto una funcion continua**, y con el producto no hay ningun problema, no va dejar de ser continua por la multiplicacion de un escalar.

**b)** Si es un subespacio, ya que tenemos el **0** porque es una funcion derivable, si sumamos dos funciones derivables, siguen siendo dervables, y lo mismo con el producto.

**c)** Este si es un subespacio contiene al **0** y a todas las funciones que tienen este tipo de forma.
$$
(2x^(-2))prime = -4x
$$

