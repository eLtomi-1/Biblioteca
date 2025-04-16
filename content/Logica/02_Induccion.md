---
title: 1- Induccion
---

## Conjuntos inductivos

Como podemos definir un conjunto, bueno hay **varias maneras** la primera de todas es por **extencion** que es la que ya conocemos.

$$
A = {0,2,4}
$$

Tambien los podemos definir por **comprension** dando una condicion que tienen que cumplir los elementos del conjunto.

$$
B = {x in NN : x "es par y" x > 5}
$$

Y la importante en este caso, por **induccion** que viene a ser mediante **reglas o clausulas**.

### Definir conjuntos por induccion

Los pasos para hacer esto serian:

1. Asumir cierto universo
2. Elegir **elementos individuales del universo** como elementos basicos del conjunto
3. Agregar **nuevos elementos** al conjunto combinando los **elementos agregados anteriormente**

Esta seria parte de la **vision constructiva**.

>[!note]-
>![Lim](2025-04-03_17-35.png)

#### Ejemplos 

Por ejemplo podriamos definir los naturales.

Indicando en que universo nos paramos, despues elegir un **elemento individual** en este caso **el 0**, y dando otra regla para **agregar nuevos elementos**, por ejemplo si tenemos $n$ le podemos sumar siempre $+1$ que va a seguir perteneciendo al conjunto.

Definimos los **naturales** $NN$ **incluido estricto** en $RR$

1. $0 in NN$
2. Si $n in NN$, entonces $n+1 in NN$

O si queremos construir un conjunto de los **pares** $PP$ **incluido estricto** en $NN$.

1. $0 in PP$
2. Si $n in P$, entonces $n+2 in PP$ 

Aca el elemento **base** seria ${0}$.

#### Comparacion

Ahora definamos $PP prime$ 

1. $0 in PP prime$
2. $2 in PP prime$
3. Si $n in PP prime$, entonces $n+4 in PP$

El conjunto base de este es ${0,2}$

Pero ahora la parte **importante**, si nos damos cuenta, tienen maneras distintas de llegar al mismo resultado, ya que tenemos dos bases distintas.

Imaginemos que queremos ver quien llega mas rapido al **numero 10**, $PP prime$ siempre va a llegar mas rapido porque hace menos pasos, empieza en el **2** salta al **6** y depues al **10**, resumiendo **3 pasos** sin embargo $P$ hubiera tardado **5 pasos**.

En terminos de computacion es **mas rapido** $$PP prime$$.

### Lenguajes

Los lenguajes estan compuestos por:

1. **Sintaxis**, compuesto por un conjunto de **simbolos**, **alfabeto** y un **conjunto de relgas**.

2. **Semantica**,

3. **Interpretacion**, un mecanismo donde de le asigna a cada frase correcta se le asigna un significado


### Universo de las palabras $Sigma$

Sea $Sigma$ un conjunto conocido de cosas distinguibles (simbolos, letras , marcaso)

Una palabra (string, tira, etc), sobre $Sigma$ es una **secuencia finita** de elementos de $Sigma$

Dadas **dos palabras** $u,w$ la palabra $u w$ es la que resulta de concatenar ambas.

Existe $epsilon$ que no tiene ninguna letra y es el **string vacio**.

Llamamos $Sigma^*$ al conjunto de todas las palabras formadas por $Sigma$

>[!important]
> Hay lenguajes que se pueden definir inductivamente y tratar como conjuntos inductivos.

#### Ejemplos

Vamos a definir $L$ de Lenguaje.

$L_1 subset.eq {a,b}^*$

1. $a in L_1$

2. Si $w in L_1$ entonces $b w b in L_1$ 

Este conjunto representa las **tiras** que tienen una sola $a$ y la misma cantidad de $b$ antes y despues de la $a$.

Este tambien se puede **definir inductivamente**:

1. Tenemos el alfabeto ${a,b}$

2. Definimos inductivamente $S subset.eq {a,b}^*$ con las siguientes reglas:
    
    - $epsilon in S$ (empty string)
    - Si $w in S$, entonces $a w in S$
    - Si $w in S$, entonces $b w in S$

    
## Pruebas inductivas

Como podriamos hacer **pruebas inductivas**, es decir **probar** que un **elemento pertenece** a ese conjunto, bueno en realidad nosotros sabemos como se **construye** cada uno de estos **conjuntos inductivos** asi que con eso deberia de ser suficiente.

Queremos probar que todos los elementos de $L_1$ tienen una **cantidad impar de simbolos**, $a$ tiene una cantidad impar de simbolos, si $w$ tambien tiene una cantidad impar de simbolos significa que $b w b$ tambien por lo tanto se cumple.

### PIP (Principio de induccion primitiva)

Un ejemplo de principio de induccion primitva es:

$NN subset.eq RR$ definido inductivamente por:

1. $0 in NN$
2. Si $n in NN$, entonces $S(n) in NN$

$S(n)$ perfectamente podria ser $n + 1$.

#### Principio de induccion primitiva para $NN$

Sea $P$ una propiedad sobre los elementos de $NN$ que cumplen lo siguiente:

1. $P(0)$ se cumple 
2. Si $n in NN$ y $P(n)$ se cumple, entonces $P(S(n))$ se cumple.

Entonces todos los elementos de $NN$ cumplen $P$.

Ahora queremos **probarlo** con este principio.

Primero la **hipostesis**.

#### **Hipotesis:**

Sea $P$ una propiedad sobre los elementos de $NN$ que cumplen lo siguiente:

1. $P(0)$ se cumple 
2. Si $n in NN$ y $P(n)$ se cumple, entonces $P(S(n))$ se cumple.

Entonces todos los elementos de $NN$ cumplen $P$.

#### **Tesis:**

**Demo**

$P$ se cumple para cualquier elemento de $NN$

1. Sea $X = {x in NN | P(x)}$
2. Por hipotesis, $X$ cumple las reglas 1 y 2 que definen a $NN$.
3. Como $NN$ es el minimo conjunto que cumple con esas reglas entonces $NN subset.eq X$
4. Entonces todos los naturales cumplen $P$.

Para dar una mejor explicacion de esto, en $P(x)$ esta incluido el **0** por lo tanto va a estar $P(0)$ que se va a cumplir por la **hipotesis** y ademas tambien $P(x)$ esta incluida la segunda regla que es $P(n)$ que $P(n) = P(x)$.

### Resumen

Resumiendo primero tenemos que probar las reglas base, en el caso de **los naturales** seria que $0 in NN$, despues seria con probar los **constructores** del conjunto inductivo como podria ser $n+1 in NN$.




