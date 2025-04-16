---
title: 3- Logica Proposicional
---

En este caso tenemos y generamos un alfabeto del lenguaje llamado $Sigma_"PROP"$ que consiste de:

1. Letras proposicionales $P = {p, q, dot dot dot}$

2. Conectivos $C = C_0 union C_1 union C_2$ y $C_0 = {bot}, C_1 = {not}, C_2 = {and, or, arrow, arrow.r.l}$

3. Simbolos auxiliares $A = {(,)}$

### Ejemplos 

Ahora vamos a traducir varias proposiciones a **PROP**.

Vamos a poner varias de ejemplo:

- Ayer llovio $(p_1)$
- El sol gira $(p_2)$
- 2 es par $(p_3)$

Ahora vamos a combinar esto con los **conectores logicos**.

- Ayer llovio **entonces** el sol gira $(p_1 arrow p_2)$
- Ayer llovio **y** 2 es par $(p_1 and p_2)$
- El sol **no** gira $(not p_2)$

### Definicion inductiva de PROP

1. Si $p in P$, entonces $p in "PROP"$
2. $bot in "PROP"$ 
3. Si $alpha in "PROP", beta in "PROP"$, entonces
    - $(alpha and beta) in "PROP"$
    - $(alpha or beta) in "PROP"$
    - $(alpha arrow beta) in "PROP"$
    - $(alpha arrow.r.l beta) in "PROP"$
4. Si $alpha in "PROP"$, tambien $not alpha in "PROP"$.

### Conversiones sintacticas

- Los conectivos $and$ y $or$ tienen el mismo nivel
- Los conectivos $arrow$ y $arrow.r.l$ tienen el mismo nivel y el **menor** nivel de todos
- El conectivo $not$ tiene el **mayor** nivel de todos

Ejemplos:
![Ejemplos](2025-04-16_16-57.png)

