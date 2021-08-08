---
layout: default
title: Premiers résultats de théorie des ensembles
language: fr
handle: /set_res1
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Ensemble de compréhension
Si $$a$$ est un ensemble et $$P$$ est une propriété, l'unique ensemble $$b$$ des éléments de $$a$$ vérifiant $$P$$ est un sous-ensemble de $$a$$.

**Preuve.** Si $$x$$ est un ensemble appartenant à $$b$$, alors $$x$$ est un ensemble appartenant à $$a$$ vérifiant la propriété $$P$$, donc $$x \in a$$. On a donc bien $$x \in b \implies x \in a$$, d'où $$b \subseteq a$$.

### Union de deux ensembles
Si $$a$$ et $$b$$ sont deux ensembles, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « $$x \in a \lor x \in b$$ ». On l'appelle l'**union** de $$a$$ et de $$b$$ et on le note $$a \cup b$$.

**Preuve.** D'après l'axiome de la paire, il existe l'ensemble $$p = \{ a, b \}$$. D'après l'axiome de la réunion, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « il existe $$y \in p$$ tel que $$x \in y$$ ». Cette dernière affirmation étant encore équivalente à « $$x \in a \lor x \in b$$ », cela conclut.

### Intersection de deux ensembles
Si $$a$$ et $$b$$ sont deux ensembles, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « $$x \in a \land x \in b$$ ». On l'appelle l'**intersection** de $$a$$ et de $$b$$ et on le note $$a \cap b$$.

**Preuve.** Notons $$P$$ la propriété d'appartenance à l'ensemble $$b$$. D'après l'axiome de compréhension, il existe un unique sous-ensemble $$c \subseteq a$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre les affirmations « $$x \in c$$ » et « $$x \in a \land  x$$ vérifie $$P$$ ». Cette dernière affirmation étant encore équivalente à « $$x \in a \land x \in b$$ », cela conclut.

### Ensemble vide
Il existe un unique ensemble ne contenant aucun élément. On l'appelle l'**ensemble vide** et on le note $$\varnothing$$.

**Preuve.** Soit $$a$$ un ensemble et notons $$P$$ la propriété de non-appartenance à $$a$$. D'après l'axiome de compréhension, il existe un unique sous-ensemble $$b \in a$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre les affirmations « $$x \in b$$ » et « $$x \in a \land  x$$ vérifie $$P$$ ». Cette dernière affirmation est donc équivalente à « $$x \in a \land x \notin a$$ », laquelle est toujours fausse puisqu'elle est de la forme $$Q \land \overline Q$$. Nous avons donc montré l'existe d'un unique ensemble $$b$$ tel que pour tout ensemble $$x$$, on ait $$x \notin b$$.

### Couple d'ensembles
Si $$a$$ et $$b$$ sont deux ensembles, on appelle **couple** de $$a$$ et $$b$$ l'ensemble $$\{ \{ a \}, \{ a, b \} \}$$ et on le note $$(a, b)$$.

**Preuve.** Nous n'avons qu'à montrer l'existence de cet ensemble. L'axiome de la paire validant l'existence des ensembles $$\{ a \}$$ et $$\{a, b \}$$, on l'applique une troisième fois avec ces deux derniers pour obtenir l'existence de l'ensemble donné dans l'énoncé.

### Produit cartésien de deux ensembles
Etant donnés deux ensembles $$a$$ et $$b$$, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$z$$, il  y ait équivalence entre les affirmations « $$z \in c$$ » et « il existe $$x \in a$$ et $$y \in b$$ tel que $$z = (x, y)$$ ».

**Preuve.**
