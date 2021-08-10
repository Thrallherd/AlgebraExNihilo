---
layout: default
title: Définition des fonctions
language: fr
handle: /set_res2
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Couple d'ensembles
Si $$a$$ et $$b$$ sont deux ensembles, on appelle **couple** de $$a$$ et $$b$$ l'ensemble $$\{ \{ a \}, \{ a, b \} \}$$ et on le note $$(a, b)$$.

**Preuve.** Nous n'avons qu'à montrer l'existence de cet ensemble. L'axiome de la paire validant l'existence des ensembles $$\{ a \}$$ et $$\{a, b \}$$, on l'applique une troisième fois avec ces deux derniers pour obtenir l'existence de l'ensemble donné dans l'énoncé.

### Unicité des couples
Si $$a$$, $$b$$, $$c$$ et $$d$$ sont quatre ensembles, il y a équivalence entre les deux affirmations « $$(a, b) = (c, d)$$ » et « $$a = c \land b = d$$ ».

**Preuve.** Si $$a = c \land b = d$$, alors d'une part on a $$\{ a \} = \{ c \}$$ et d'autre part $$\{a, b\} = \{c, d\}$$. Il y a inclusion réciproque entre les ensembles $$\{ \{ a \}, \{ a, b \} \}$$ et $$\{ \{ c \}, \{ c, d \} \}$$, ils sont donc égaux. Réciproquement si ces ensembles sont égaux, nous allons faire une disjonction de cas. 

* Si $$a = b$$, alors $$(a, b)$$ est un ensemble à un élément : le singleton $$\{ a \}$$. Il en va donc de même pour l'ensemble $$(c, d)$$, donc les ensembles $$\{ c \}$$ et $$\{ c, d \}$$ sont égaux. Si $$d \neq c$$, $$\{ c, d \}$$ et donc $$\{ c \}$$ contiendraient deux éléments. On conclut par l'absurde que $$c = d$$.

* Si $$a \neq b$$, alors $$(a, b)$$ est un ensemble à deux éléments. Il en va donc de même pour l'ensemble $$(c, d)$$. Par inclusion de $$(a, b)$$ dans $$(c, d)$$, on a donc $$\{ a \} \in \{ \{ c \}, \{ c, d \} \}$$. Si $$ \{ a \} = \{ c, d \}$$, un ensemble à un élément serait égal à un ensemble à deux éléments, ce qui n'est pas possible, donc $$\{ a \} \neq \{ c, d \}$$. Si $$\{ a \} \neq \{ c \}$$ non plus, alors $$\{ a \} \notin (c, d)$$. On conclut donc par l'absurde que $$\{ a \} = \{ c \}$$, soit finalement $$a = c$$. Comme $$\{ a, b \} \neq \{ a \}$$, si $$\{ a, b \} \neq \{ c, d \}$$ on aurait alors $$\{ a, b \} \notin (c, d)$$, ce qui est exclu. On a donc $$\{ a, b \} = \{ c, d \}$$ par l'absurde. Comme $$b \in \{ c, d \}$$, si $$b = c$$, alors $$b = a$$ qui est faux. On a donc par l'absurde $$b = d$$.

### Produit cartésien de deux ensembles
Etant donnés deux ensembles $$a$$ et $$b$$, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$z$$, il  y ait équivalence entre les affirmations « $$z \in c$$ » et « il existe $$x \in a$$ et $$y \in b$$ tel que $$z = (x, y)$$ ». On appelle cet ensemble le **produit cartésien** de $$a$$ et de $$b$$, et on le note $$a \times b$$.

**Preuve.** Notons $$u$$ l'ensemble des parties de $$a \cup b$$ et $$P$$ la propriété d'être égal à un couple $$(x, y)$$ tel que $$x \in a$$ et $$y \in b$$. D'après l'axiome de compréhension, il existe un unique sous-ensemble $$c \subseteq u$$ tel qu'il  y ait équivalence entre les affirmations « $$z \in c$$ » et « $$z \in u \land z$$ vérifie $$P$$ ». Cette dernière affirmation est équivalente à « $$z \in u~\land$$ il existe $$x \in a$$ et $$y \in b$$ tel que $$z = (x, y)$$ ». Le fait que $$z$$ soit le couple d'un élément de $$a$$ et d'un élément de $$b$$ impose *de facto* que $$z$$ appartienne à $$u$$, on conclut donc qu'il y a équivalence entre les affirmations « $$z \in c$$ » et « il existe $$x \in a$$ et $$y \in b$$ tel que $$z = (x, y)$$ ».

### Triplet d'ensembles
Si $$a$$, $$b$$ et $$c$$ sont trois ensembles, on appelle **triplet** de $$a$$, $$b$$ et $$c$$ le couple $$((a, b), c)$$, c'est-à-dire l'ensemble $$\{ \{ (a, b) \}, \{ (a, b), c \} \}$$ et on le note $$(a, b, c)$$.

### Unicité des triplets
Si $$a$$, $$b$$, $$c$$, $$x$$, $$y$$ et $$z$$ sont six ensembles, il y a équivalence entre les deux affirmations « $$(a, b, c) = (x, y, z)$$ » et « $$a = x \land b = y \land c = z$$ ».

**Preuve.** Si $$(a, b, c) = (x, y, z)$$, alors par définition on a $$((a, b), c) = ((x, y), z)$$. Par unicité des couples, on a donc $$(a, b) = (x, y)$$ et $$c = z$$, soit encore $$a = x$$, $$b = y$$ et $$c = z$$. Réciproquement si nous avons ces trois égalités, alors $$(a, b) = (x, y)$$, et par unicité des couples, on a bien $$((a, b), c) = ((x, y), z)$$, ce qui conclut.

### Produit cartésien de trois ensembles
On appelle **produit cartésien** de trois ensembles $$a$$, $$b$$ et $$c$$ l'ensemble $$(a \times b) \times c$$. C'est l'ensemble de tous les triplets $$(x, y, z)$$ tels que $$x \in a \land y \in b \land z \in c$$. Par abus, on note cet ensemble $$a \times b \times c$$.

### Carte entre deux ensembles (terme propre à ce site)
On dit que l'ensemble $$c$$ est une **carte** de l'ensemble $$a$$ vers l'ensemble $$b$$ lorsque $$c \subseteq a \times b$$ et si pour tout ensemble $$x \in a$$ et $$y, z \in b$$, il y a équivalence entre les affirmations « $$(x, y) \in c \land (x, z) \in c$$ » et « $$y = z$$ ».

### Fonction entre deux ensembles
On dit que l'ensemble $$f$$ est une **fonction** d'un ensemble $$a$$ vers un ensemble $$b$$ s'il existe une carte $$c$$ telle que $$f = a \times b \times c$$.
