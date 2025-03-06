---
title: Practico 8
---

Combinaciones lineales, dependencia e independencia lineal

> [!note] Aclaracion
> **R:** 
> Significa **R**espuesta
>
> Los **ejercicios** que no estan todos eran de **probar/demostrar**.

### 1)
![Aej1](2025-01-30_00-40.png)

**a) R: SI**; Bueno lo primero que podemos hacer para saber si el conjunto $v$ es una **combinacion lineal** es armar **un sistema**.

$$
 cases(
    lambda + 3 alpha + beta = 3 \
    2lambda - alpha + beta= 0\
    lambda + 5alpha = 6 
)
$$

Como vemos que con el sistema asi nomas no podemos resolver mucha cosa lo pasamos a una matriz.

$$
mat(1, 3, 1, 3; 2, -1, 1, 0; 1, 5, 0, 6; augment: #3)
$$

Escalarizandola nos va quedar una matriz asi:

$$
mat(1, 3, 1, 3; 0, -7, -1, -6; 0, 0, -9, 9; augment: #3)
$$

Que si lo pasamos de vuelta a sistema y lo resolvemos nos va a dar que las incognitas tiene los siguientes valores.

$$
beta = -1;space alpha = 1; space lambda = 1
$$

Como podemos ver estas son las **coordenadas** para que la **combinacion lineal de los vectores** de $A$ nos den como resultado el vector $v = (3,0,6)$

> [!note]- Dato
> En realidad si en una matriz **igualamos** un **conjunto de vectores** a un **vector** y nos da un valor para cada variable $lambda, alpha, beta$, significa que el vector es combinacion lineal del conjunto.

**b) R:SI**. Ahora como es un ejercicio del mismo estilo pero ahora son vectores de $RR^4$ haremos lo mismo.


$$
 cases(
    lambda + 2 alpha + 2 beta = 2 \
    3 lambda - 2 alpha -1 beta = 5\
    2 lambda - 5 alpha +3 beta = -4\
    lambda + 4 alpha + 6 beta = 0 
)
$$

De vuelta como podemos ver nos conviene pasarlo a matriz.

$$
mat(1,2,2,2; 3,-2,-1,5; 2,-5,3,-4; 1,4,6,0; augment:#3)
$$

Al escalarizar la matriz nos queda asi:

$$
mat(1,2,2,2; 3,-2,-1,5; 0,-9,-1,-8; 0,0,34,-34; augment:#3)
$$

Y al pasarlo a sistema nos da que si es linealmente dependiente del conjunto de vectores $A$ en las coordenadas

$$
lambda = 2; space alpha = 1; space beta = -1
$$

**c) R: SI**. Bueno lo primero que podemos hacer aca es igualarlos usando combinacion lineal de esta manera.

$$
lambda(2-x) + alpha(2x-x^2) = 6 - 5x + x^2
$$

Si desarrollamos el lado izquierdo nos va a quedar asi:

$$
(2lambda) + (-lambda + 2alpha)x + (-alpha)x^2 = 6 - 5x + x^2
$$

Si igualamos los coeficientes nos da asi: 

$$
cases(
2lambda = 6 \
-lambda + 2alpha = -5 \
-alpha = 1
)
$$

Resolviendo el sistema nos queda que:

$$
lambda = 3; space alpha = -1
$$

**d) R:NO**. Hacemos lo mismo que antes e igualamos el conjunto $A$ al vector $v$ usando la combinacion lineal.

$$
lambda (3x^3 + x) + alpha (-2x^2 + x - 1) + beta (3x^2 - 2x^2 + 2x - 1) = -3x^3 + 4x^2 + x - 2
$$

Despues desarrollamos la parte izquierda de la ecuacion:

$$
(-alpha - beta) + (lambda + alpha + 2beta)x + (-2alpha -2beta)x^2 + (3lambda + 3beta)x^3 = -3x^3 + 4x^2 + x - 2
$$

De vuelta convertimos esto en un sistema igualando los coeficientes de cada uno.

$$
cases(
3lambda + 3beta = -3\
-2alpha -2beta = 4\
lambda + alpha + 2beta = 1\
-alpha - beta = -2
)
$$

Lo pasamos a matriz:

$$
mat(3, 0, 3, -3; 0, -2, -2, 4; 1, 1, 2, 1; 0, -1, -1, -2; augment:#3)
$$

Enseguida empezamos a resolver nos damos cuenta que es una **matriz incompatible**, ya que si bien logramos **eliminar una fila porque es igual a otra** que ya existe, despues nos encontramos esta incoherencia.
$$
mat(3, 0, 3, -3; 0, 3, 3, 6; 0, 0, 0, 12; augment:#3)
$$

Claramente $0 eq.not 12$ y no es como dice la matriz. En resumen no es **linealmente dependiente** del conjunto de vectores $A$

**e) R: SI**. Primero que todo hacemos un sistema. 

$$
cases(
lambda + beta = 2\
-alpha -2beta = -1\
 alpha + 2beta = 1\
lambda + beta = 2
)
$$

Bueno es este caso tenemos un problema ya que nos da un sistema **compatible indeterminado** observemos restando algunas columnas:

$$
cases(
-alpha -2beta = -1\
lambda + beta = 2
)
$$

Como podemos ver tenemos una **variable en comun** en las dos filas y esta es $beta$. Al determinar que tiene **soluciones infinitas** el sistema podemos ver si **dandole un valor** a $beta$ nos puede dar una de esas soluciones para decidir si es combinacion lineal del conjunto

Si hacemos $beta = 0$, nos da que:

$$
beta = 0;  space alpha = 1; space lambda = 2;
$$

Esa es una combinacion lineal valida por lo tanto **si es una combinacion lineal del conjunto $A$**.

**f) R: NO**. Lo mismo, hacemos un sistema con los datos dados.

$$
cases(
2lambda + 6beta = 6\
-3lambda + 5alpha -19beta = 2\
4lambda + alpha + 10beta = 9\
lambda -2 alpha + 7beta = 11
)
$$

Como no hay nada muy claro lo pasamos a matriz:

$$
mat(2,0,6,6;-3,5,-19,2;4,1,10,9;1,-2,7,11; augment:#3)
$$

Al escalarizar la matriz nos damos cuenta de que nos da un **sistema incompatible**, resultando en que no es **linealmente dependiente** del conjunto de vectores $V$.

$$
mat(2,0,6,6;-3,5,-19,2;0,1,-2,-3;0,0,0,4; augment:#3)
$$

Claramente $0 eq.not 4$

> [!note]- Dato
> Este es un caso perfecto para ver cuando no es combinacion lineal, es **incompatible** por lo tanto no va a dar valores para las variables presentadas.

### 2)

![Aej2](2025-01-30_22-42.png)

**a)** Primero intentamos **pasar de tener 3 a 2 variables** haciendo esto $x+y+z=0$ y pasandolo a $z=-x-y$ por lo tanto cualquier vector $(x,y,z)$ sera reescrito asi $(x,y,-x-y)$.

Luego separamos los vectores que contienen el $y$ de los que contienen el $x$.

$$
(x,0,-x) + (0,y,-y)
$$

Despues sacamos las $y$ ademas de las $x$ para que nos queden los vectores como una combinacion lineal.
$$
x(1,0,-1) + y(0,1,-1)
$$

Y ahora podemos ver claramente que los vectores $G = {(1,0,-1), (0,1,-1)}$ forman un **generador finito del subespacio** $S$

**b)** Primero que todo tenemos que ver como es el polinomio $p(1-x)$ y $p(1+x)$.

$$
lambda(1-x)^3 + alpha(1-x)^2 + beta(1-x) + d = lambda(1+x)^3 + alpha(1+x)^2 + beta(1+x) + d
$$

La idea para hayar este tipo de generadores es **armar el sistema en base a los coeficientes** y agarrar las condiciones. 

$$
(lambda + alpha + beta + d) + (-beta -2 alpha -3 lambda)x + (alpha + 3lambda)x^2 + (-lambda)x^3 
$$
$$
$$
$$
= (lambda + alpha + beta + d) + (beta +2 alpha +3 lambda)x + (alpha + 3lambda)x^2 + (lambda)x^3
$$

Las condiciones que podemos sacar de aca en un sistema son asi:

$$
 cases(
    lambda + alpha + beta + d = lambda + alpha + beta + d \
    -beta -2 alpha -3 lambda = beta +2 alpha +3 lambda\
    alpha + 3lambda = alpha + 3lambda\ 
   -lambda = lambda
)
$$

De aca podemos sacar que $lambda = 0$, al cumplirse esto podemos sacar varias cosas del sistema. Ademas de las **igualdades que no nos sirven de nada**.

$$
 cases(
    -beta -2 alpha = beta +2 alpha \
   lambda = 0
)
$$

Aca sumamos en la primera fila $beta +2alpha$ y luego dividimos en $2$ para que nos quede asi.

> [!important]- Dato importante
> Cuando queremos hayar el generador es muy importante **sacarle las condiciones del sistema** como se ve aca, para despues aplicarlas en un polinomio generico. Luego **los coeficientes que quedan son lo que genera ese espacio**.

$$
 cases(
    beta +2 alpha = 0 \
   lambda = 0
)
$$

Las condiciones son $beta = -2alpha; space lambda = 0$

$$
p(x) = cancel(lambda x^3) + alpha x^2 - 2 alpha x + d
$$
$$
$$
$$
p(x) =  alpha (x^2 - 2x) + d(1)
$$

En resumen el conjunto generador es $G = {x^2 - 2x, 1}$, lo que hicimos primero fue **desarrolar el polinomio**, pasarlo a sistema, conseguir las condiciones y **aplicarlas en un polinomio generico** para sacar los coeficientes de las variables que son lo que componen al conjunto $G$

**c)** Primero ponemos el ejemplo de $p(0) = 0$

$$
lambda(0)^3 + alpha(0)^2 + beta(0) + d = 0
$$

Si nos damos cuenta, **todo se va** porque esta multiplicado por **0** menos la variable $d$. O sea que para que el poliniomio sea igual a **0**, se tiene que cumplir la condicion $d = 0$, **(que esta vez conseguimos sin sistema)**.

Pasando esto a un polinomio generico con $d=0$ **quedan asi los coeficientes**.
$$
lambda x^3 + alpha x^2 + beta x
$$

Vamos a hacer el **conjunto generador con los coeficientes de las variables $lambda, alpha, beta$**, y el conjunto queda asi $G = {x^3, x^2, x}$

#### Los demas son de matrices que ya se saben el conjunto generador de las mismas

### 3)

![Aej3](2025-01-31_03-35.png)

> [!important]- Aclaracion
> En este caso para verificar si es un generador de un espacio tenemos que lograr ver **si tiene el mismo rango que el de la dimension que genera**, ademas de verificar que es compatible determinado.

**a)** la diferencia entre para saber si es combinacion lineal o un generador, es que en el generador le ponemos el vector generico.

$$
lambda(1,pi) + alpha(sqrt(2),e) = (x,y)
$$

Lo pasamos a sistema:

$$
cases(
lambda + alpha sqrt(2) = x \
lambda pi+ alpha e = y
)
$$

Lo pasamos a matriz ya que no hay ninguna solucion evidente.

$$
mat(1,sqrt(2), x; pi,e,y; augment: #2)
$$

Escalarizamos:

$$
mat(1,sqrt(2), x; 0,e-pi sqrt(2),y- pi x; augment: #2)
$$

Como podemos ver tiene rango 2, eso significa que es un generador, en general si lo podes convertir en matriz y da el rango que tiene que sar **significa que es un generador**.

**b)** Ahora con este hacemos lo mismo, diria que lo pasemos directo a matriz.

$$
mat(0,0,1,1,x; 1,0,1,-1,y; 1,1,1,1,z; augment:#4)
$$

Interacambiamos la primera y la ultima fila:

$$
mat(1,1,1,1,z; 0,-1,0,-2,y-z; 0,0,1,1,x; augment:#4)
$$

Como nos damos cuenta **escalarizada tiene rango 3** asi que en efecto es un generador de $RR^3$

**c)** Oh no!, tenemos que hacer lo mismo.

$$
mat(-1,2,3,0,x; 2,0,0,0,y; 0,-1,0,5,z;0,0,4,0,w; augment:#4)
$$

Escalarizamos para ver si tiene rango 4:

$$
mat(-1,2,3,0,x; 0,4,6,0,y+2x; 0,0,6,20,4z+y+2x;0,0,0,-80,6w-(16z+4y+8z); augment:#4)
$$

Efectivamente **lo tiene asi que es un generador de** $RR^4$

**d)** Oh no! De vuelta!, nada mas que ahora el general de las matrices de $2 times 2$ es $mat(a,b;c,d)$

$$
mat(2,0,3,0,a; 1,0,-1,0,b; 0,2,0,3,c;0,1,0,1,d; augment:#4)
$$

Aca esta escalarizada (cabe que me olvide calcular a lo que estan igualadas las ecuaciones es decir las variables)

$$
mat(2,0,3,0,?; 0,1,0,1,?; 0,0,-5,0,?;0,0,0,1,?; augment:#4)
$$

Resumiendo aunque aun no dimos teorema de las dimensiones, **es un generador ya que el rango de la matriz es 4**.

**e)** Bueno ahora definitivamente no tenemos que hacer lo mismo pero algo parecido.

$$
lambda(x-2)^2 + alpha(x-2) + beta = lambda x^2 + alpha x + beta 
$$
$$
$$
$$
lambda(x^2-4x+4) + alpha(x-2) + beta = lambda x^2 + alpha x + beta 
$$

Ahora pasamos a sistema:

$$
 cases(
    x^2 -4x + 4 = x^2 \
    2x - 2 = x\
     1 = 1
)
$$

Bueno si nos damos cuenta esto ya es un a matriz escalarizada y con rango 3, por lo tanto si es un generador de $RR_2 [x]$

### 4)
![Aej4](2025-02-02_22-00.png)

Tenemos varias maneras de ir verificando y descartando. La primera **es saber si los subespacios que generan tienen la misma dimension**. Para eso tenemos que escalarizar en este caso el conjunto $A_1$.

$$
mat(1,0,2,x;2,1,5,y;-1,1,-1,z; augment:#3) arrow.r.double.long mat(1,0,2,x;0,1,1,y -2z;0,0,0,x+y+z; augment:#3)
$$

Bueno nos damos cuenta que tiene **rango igual 2** por lo tanto los dos conjuntos generan el mismo espacio, y **hay un vector de mas** que en este caso es el $(2,5,-1)$ el cual podemos **ignorar**.

Ahora tenemos que ver si con los vectores de $A_2$ podemos construir los vectores de $A_1$ y viceversa.

$$
alpha(-2,-6,0) + beta(1,1,-2) = (1,2,-1)
$$ 
$$ 
$$ 
$$
alpha(-2,-6,0) + beta(1,1,-2) = (0,1,1)
$$

Si hacemos el sistema:

$$
 cases(
    -2alpha + beta = 1 \
    -6alpha + beta = 2\
    -2 beta = -1
)
$$

Resolviendo este sistema nos da estos valores $alpha= -1/4; beta=1/2$.

$$
 cases(
    -2alpha + beta = 0 \
    -6alpha + beta = 1\
    -2 beta = 1
)
$$

Resolviendo este sistema nos da estos valores $alpha= -3/4; beta=-1/2$. 

Como podemos ver efectivamente podemos generar los vectores de $A_1$ con los vectores de $A_2$

$$
-1/4(-2,-6,0) + 1/2(1,1,-2) = (1,2,-1)
$$ 
$$ 
$$ 
$$
-3/4(-2,-6,0) + -1/2(1,1,-2) = (0,1,1)
$$

y **viceversa** como se muestra aca.
![Aaej4](2025-02-03_00-47.png)

**En conclusion, si generan el mismo espacio**


### 5)
![Aej5](2025-02-03_01-24.png)
![Aaej5](2025-02-03_01-25.png)

**a)** Primero juntamos los vectores en una matriz, y la **escalarizamos** para ver que vectores "sobran" y cuales no.

Al escalarizarla quedan **solo los vectores que son linealmente independientes**.

$$
mat(1,2,3;0,1,2;0,-1,-2;0,0,0) arrow.r.double.long mat(1,2,3;0,1,2;0,0,0;0,0,0)
$$

Cuando escalarizamos esta matriz los vectores **no independientes** quedaron en **0** y los vectores **independientes** son los que estan aun en la matriz.

Por lo tanto no es un **conjunto linealmente independiente** y el **subconjunto linealmente independiente** es $I = {(1,2,3),(0,1,2)}$

**b)** Hacemos lo mismo, pasar el **conjunto a matriz**.

$$
mat(4,0,-2,-2;1,-1,2,3;0,2,1,4;-1,5,7,1) arrow.r.double.long mat(4,0,-2,-2;0,-4,10,14;0,0,7,15;0,0,0,13)
$$

Como podemos ver el **rango es 4** el cual tambien es la **dimension del espacio en el que se encuentra**, y ningun vector quedo en **0** por lo tanto es un conjunto **linealmente independiente**.

**c)** Bueno, ahora que es de polinimio, primero lo tenemos que desarrolar.

$$
lambda(x^2+1) + alpha(x^2+x) + beta(x+2) + d(x^2+3)
$$
$$
$$
$$
arrow.b.double
$$
$$
(lambda + 2beta) + (alpha + beta + 3d)x + (alpha + d + lambda)x^2
$$

Ahora que ya lo tenemos desarrolado podemos pasar esto a una matriz.

$$
mat(1,0,1;2,1,0;0,1,1;0,3,1) arrow.r.double.long mat(1,0,1;0,1,0;0,0,1;0,0,0)
$$

El que estaba ultimo es el que quedo en **0** por eso mismo el conjunto **no era linealmente independiente**, el subconjunto que si cumple para ser **linealmente independiente** es $I ={(1,0,1),(2,1,0),(0,1,1)}$.

O mejor dicho $I = {x^2+1 ,x^2 + x, x + 2}$ sin $x^2+3$

### 6)

![Aej6](2025-02-03_04-15.png)

**a)** Primero que todo le vamos a hacer el determinante, asi vamos a saber en que casos es **linealmente dependiente o linealmente independiente**.

$$
A = mat(a,-1,0;a^2,a,2a^2;1,a,a^2+1)
$$

El determinante da como resultado $det(A) = a^4+a^2-2a^2-2a^4+a^4+a^2 = 0$ por lo tanto el conjunto dado es siempre **linealmente dependiente** sin importar el valor de $a$.

**b)** Bueno al tener una variable $a$ lo ideal seria hacerle **el determinante** para saber si es **linealmente independiente**.

Hacemos una matriz en base a los vectores del conjunto.

$$
A = mat(1,-1,2;1,a,1;a,1,3)
$$

Hacemos el determinante $det(A) = -2a^2+2a+4$, como nos damos cuenta **depende de** $a$, y tenemos que ver cuando es **0** para saber cuando es **linealmente dependiente**, asi que al ser un **polinomio de grado 2** aplicamos bhaskara.

Nos da que cuando $a=2$ o $a=-1$ el conjunto en **linealmente dependiente** es decir da **0**. Pero en todos los demas casos es **linealmente independiente**

### 7)

![Aej7](2025-02-04_21-07.png)

Podriamos hacer varias cosas, pero para mi la mas inteligente seria pasarlo a una matriz directamente.

$$
mat(1,0,0,3;0,1,-1,-1;-1,-1,0,-2;0,2,-1,1) arrow.r.double.long mat(1,0,0,3;0,1,-1,-1;0,0,-1,0;0,0,0,3)
$$

Al escalarizarla completamente nos damos cuenta que es **linealmente independiente** y no sobra ningun vector. A todo esto tiene **rango igual a 4**, por lo tanto **genera el espacio vectorial** de las matrices $2 times 2$.

>[!note] Aclaracion
>Al ser el **rango de la matriz igual a 4**, significa que genera un **espacio de dimension 4**. Al estar hablando de matrices esto significa que **genera un espacio vectorial de matrices** de dimension 4. Que es igual al de las matrices $2 times 2$

### 8)

![Aej8](2025-02-04_22-17.png)

**a)** Que $C$ sea **linealmente independiente no asegura en ningun momento** que $B$ lo sea, ya que podemos modificar $B$ con cualquier matriz posible para que sea **linealmente dependiente**.

Por lo tanto es **falsa**.

**b)** Sin embargo si $B$ es linealmente independiente, si siginifica que $C$ tambien lo es, **ya que podemos multiplicar a los vectores** de $C$ por el **neutro de una matriz y que quede exactamente igual** significando que $C$ era linealmente independiente.

Por lo tanto es **verdadera**.

**c)** **No podemos** hacer a $B$ **linealmente independiente** multiplicando, si no **sacando los vectores que son linealmente dependientes**. Asi que si $C$ es linealmente dependiente, no nos queda mas remedio que $B$ **tambien lo sea**.

Por lo tanto es **verdadera**.




