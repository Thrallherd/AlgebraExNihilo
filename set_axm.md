---
layout: default
title: Axiomes de théorie des ensembles
language: fr
handle: /set_axm
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Axiome d'extensionnalité
Il n'existe pas d'ensembles distincts qui ont les mêmes éléments. Autrement dit, si $$x$$ et $$y$$ sont deux ensembles, il y a équivalence entre l'affirmation « $$x = y$$ » et l'affirmation « pour tout ensemble $$z$$, on a $$z \in x \iff z \in y$$ ».

### Axiome de la paire
Etant donnés deux ensembles $$a$$ et $$b$$, il existe un ensemble $$c$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in c$$ » et l'affirmation « $$x = a \lor x = b$$ ». L'axiome d'extensionnalité montre alors que $$c$$ est unique. L'ensemble $$c$$ est noté $$\{ a, b \}$$ et est appelé **paire** lorsque $$a \neq b$$. Dans le cas particulier où $$a = b$$, $$c$$ est appelé **singleton** et est noté simplement $$\{ a \}$$.

### Axiome de compréhension
Pour tout ensemble $$a$$ et pour toute propriété $$P$$, il existe un sous-ensemble $$b$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in b$$ » et l'affirmation « $$x \in a \land x$$ vérifie $$P$$ ». L'axiome d'extensionnalité montre alors que $$b$$ est unique.

### Axiome de la réunion
Pour tout ensemble $$a$$, il existe un ensemble $$b$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in b$$ » et l'affirmation « il existe un ensemble $$y \in a$$ tel que $$x \in y$$ ». L'axiome d'extensionnalité montre alors que $$b$$ est unique.

### Axiome de l'ensemble des parties
Pour tout ensemble $$a$$, il existe un ensemble $$b$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre l'affirmation « $$x \in b$$ » et l'affirmation « $$x \subseteq a$$ ». L'axiome d'extensionnalité montre alors que $$b$$ est unique.
