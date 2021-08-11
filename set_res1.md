---
layout: default
title: Premiers résultats de théorie des ensembles
language: fr
handle: /set_res1
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Egalité par double inclusion
Si $$a$$ et $$b$$ sont deux ensembles, on a l'équivalence $$a = b \iff a \subseteq b \land b \subseteq a$$.

**Preuve.** Si $$a = b$$, alors pour tout ensemble $$x \in a$$, on a également $$x \in b$$. L'implication $$x \in a \implies x \in b$$ est donc vérifiée, et on a $$a \subseteq b$$. On montre de la même manière que $$b \subseteq a$$, ainsi $$a = b \implies a \subseteq b \land b \subseteq a$$. Réciproquement s'il y a double inclusion, alors pour tout ensemble $$x$$ il y a équivalence entre les affirmations « $$x \in a$$ » et « $$x \in b$$ ». L'axiome d'extensionnalité montre alors que $$a = b$$.

### Unicité des singletons
Si $$a$$ et $$b$$ sont deux ensembles, on a l'équivalence $$a = b \iff \{ a \} = \{ b \}$$.

**Preuve.** Si $$a = b$$, alors les ensembles $$\{ a \}$$ et $$\{ b \}$$ désignent le même ensemble : l'ensemble contenant $$a$$ et lui seulement. On a donc $$\{ a \} = \{ b \}$$. Réciproquement si $$\{ a \} = \{ b \}$$, alors $$a \in \{ b \}$$, donc $$a = b$$.

### Ensemble de compréhension
Si $$a$$ est un ensemble et $$P$$ est une propriété, l'unique ensemble $$b$$ des éléments de $$a$$ vérifiant $$P$$ est un sous-ensemble de $$a$$.

**Preuve.** Si $$x$$ est un ensemble appartenant à $$b$$, alors $$x$$ est un ensemble appartenant à $$a$$ vérifiant la propriété $$P$$, donc $$x \in a$$. On a donc bien $$x \in b \implies x \in a$$, d'où $$b \subseteq a$$.

### Ensemble vide
Il existe un unique ensemble ne contenant aucun élément. On l'appelle l'**ensemble vide** et on le note $$\varnothing$$.

**Preuve.** Soit $$a$$ un ensemble et notons $$P$$ la propriété de non-appartenance à $$a$$. D'après l'axiome de compréhension, il existe un unique sous-ensemble $$b \subseteq a$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre les affirmations « $$x \in b$$ » et « $$x \in a \land  x$$ vérifie $$P$$ ». Cette dernière affirmation est donc équivalente à « $$x \in a \land x \notin a$$ », laquelle est toujours fausse puisqu'elle est de la forme $$Q \land \overline Q$$. Nous avons donc montré l'existe d'un unique ensemble $$b$$ tel que pour tout ensemble $$x$$, on ait $$x \notin b$$.

### Union de deux ensembles
Si $$a$$ et $$b$$ sont deux ensembles, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « $$x \in a \lor x \in b$$ ». On l'appelle l'**union** de $$a$$ et de $$b$$ et on le note $$a \cup b$$.

**Preuve.** D'après l'axiome de la paire, il existe l'ensemble $$p = \{ a, b \}$$. D'après l'axiome de la réunion, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « il existe $$y \in p$$ tel que $$x \in y$$ ». Cette dernière affirmation étant encore équivalente à « $$x \in a \lor x \in b$$ », cela conclut.

### Intersection de deux ensembles
Si $$a$$ et $$b$$ sont deux ensembles, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « $$x \in a \land x \in b$$ ». On l'appelle l'**intersection** de $$a$$ et de $$b$$ et on le note $$a \cap b$$.

**Preuve.** Notons $$P$$ la propriété d'appartenance à l'ensemble $$b$$. D'après l'axiome de compréhension, il existe un unique sous-ensemble $$c \subseteq a$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre les affirmations « $$x \in c$$ » et « $$x \in a \land  x$$ vérifie $$P$$ ». Cette dernière affirmation étant encore équivalente à « $$x \in a \land x \in b$$ », cela conclut.

### Couple d'ensembles
Si $$a$$ et $$b$$ sont deux ensembles, on appelle **couple** de $$a$$ et $$b$$ l'ensemble $$\{ \{ a \}, \{ a, b \} \}$$ et on le note $$(a, b)$$.

**Preuve.** Nous n'avons qu'à montrer l'existence de cet ensemble. L'axiome de la paire validant l'existence des ensembles $$\{ a \}$$ et $$\{a, b \}$$, on l'applique une troisième fois avec ces deux derniers pour obtenir l'existence de l'ensemble donné dans l'énoncé.

### Unicité des couples
Si $$a$$, $$b$$, $$c$$ et $$d$$ sont quatre ensembles, il y a équivalence entre les deux affirmations « $$(a, b) = (c, d)$$ » et « $$a = c \land b = d$$ ».

**Preuve.** Si $$a = c \land b = d$$, alors d'une part on a $$\{ a \} = \{ c \}$$ et d'autre part $$\{a, b\} = \{c, d\}$$. Il y a inclusion réciproque entre les ensembles $$\{ \{ a \}, \{ a, b \} \}$$ et $$\{ \{ c \}, \{ c, d \} \}$$, ils sont donc égaux. Réciproquement si ces ensembles sont égaux, nous allons faire une disjonction de cas. 

* Si $$a = b$$, alors $$(a, b)$$ est un ensemble à un élément : le singleton $$\{ a \}$$. Il en va donc de même pour l'ensemble $$(c, d)$$, donc les ensembles $$\{ c \}$$ et $$\{ c, d \}$$ sont égaux. Si $$d \neq c$$, $$\{ c, d \}$$ et donc $$\{ c \}$$ contiendraient deux éléments. On conclut par l'absurde que $$c = d$$.

* Si $$a \neq b$$, alors $$(a, b)$$ est un ensemble à deux éléments. Il en va donc de même pour l'ensemble $$(c, d)$$. Par inclusion de $$(a, b)$$ dans $$(c, d)$$, on a donc $$\{ a \} \in \{ \{ c \}, \{ c, d \} \}$$. Si $$ \{ a \} = \{ c, d \}$$, un ensemble à un élément serait égal à un ensemble à deux éléments, ce qui n'est pas possible, donc $$\{ a \} \neq \{ c, d \}$$. Si $$\{ a \} \neq \{ c \}$$ non plus, alors $$\{ a \} \notin (c, d)$$. On conclut donc par l'absurde que $$\{ a \} = \{ c \}$$, soit finalement $$a = c$$. Comme $$\{ a, b \} \neq \{ a \}$$, si $$\{ a, b \} \neq \{ c, d \}$$ on aurait alors $$\{ a, b \} \notin (c, d)$$, ce qui est exclu. On a donc $$\{ a, b \} = \{ c, d \}$$ par l'absurde. Comme $$b \in \{ c, d \}$$, si $$b = c$$, alors $$b = a$$ qui est faux. On a donc par l'absurde $$b = d$$.
