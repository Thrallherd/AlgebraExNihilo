---
layout: default
title: Premiers résultats de théorie des ensembles
language: fr
handle: /set_res1
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

A partir des [cinq premiers axiomes](set_axm.md), nous pouvons apporter quelques premiers résultats.

### Union de deux ensembles
Si $$a$$ et $$b$$ sont deux ensembles, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « $$x \in a \lor x \in b$$ ». Cet ensemble $$c$$ est noté $$a \cup b$$.

**Preuve.** D'après l'axiome de la paire, il existe l'ensemble $$p = \{ a, b \}$$. D'après l'axiome de la réunion, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « il existe $$y \in p$$ tel que $$x \in y$$ ». Cette dernière affirmation étant encore équivalente à « $$x \in a \lor x \in b$$ », cela conclut.

### Intersection de deux ensembles
Si $$a$$ et $$b$$ sont deux ensembles, il existe un unique ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « $$x \in a \land x \in b$$ ». Cet ensemble $$c$$ est noté $$a \cap b$$.

**Preuve.** Notons $$P$$ la propriété d'appartenance à l'ensemble $$b$$. D'après l'axiome de compréhension, il existe un unique sous-ensemble $$c \subseteq a$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre les affirmations « $$x \in c$$ » et « $$x \in a \land  x$$ vérifie $$P$$ ». Cette dernière affirmation étant encore équivalente à « $$x \in a \land x \in b$$ », cela conclut.
