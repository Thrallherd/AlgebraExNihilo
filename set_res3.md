---
layout: default
title: Axiome de l'ensemble des parties et conséquences
language: fr
handle: /set_res3
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Axiome de l'ensemble des parties
Pour tout ensemble $$a$$, il existe un ensemble $$b$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in b$$ » et l'affirmation « $$x \subseteq a$$ ». L'axiome d'extensionnalité montre alors que $$b$$ est unique.

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
