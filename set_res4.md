---
layout: default
title: Fonctions et résultats généraux
language: fr
handle: /set_res4
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Table entre deux ensembles (terme propre à ce site)
On dit que l'ensemble $$c$$ est une **table** de l'ensemble $$a$$ vers l'ensemble $$b$$ si on a l'inclusion $$c \subseteq a \times b$$ et si pour tout ensemble $$x \in a$$ et $$y, z \in b$$, on a l'implication $$(x, y) \in c \land (x, z) \in c \implies y = z$$.

### Fonction entre deux ensembles
On dit que l'ensemble $$f$$ est une **fonction** d'un ensemble $$a$$ vers un ensemble $$b$$ s'il existe une table $$c$$ de $$a$$ vers $$b$$ telle que $$f = (a, b, c)$$, et on note dans ce cas $$f : a \to b$$. Pour tout ensemble $$x \in a$$, s'il existe $$y \in b$$ tel que $$(x, y) \in c$$, alors $$y$$ est unique (par définition d'une table) et on le notera $$f(x)$$.

### Ensemble de définition
Soit $$f : a \to b$$. On appelle **ensemble de définition** de la fonction $$f$$ l'ensemble $$d \subseteq a$$ tel que pour tout $$x \in d$$, il existe $$y \in b$$ tel que $$f(x) = y$$.

**Preuve.** Il faut montrer ici que $$d$$ existe et est un ensemble. Soit $$c \subseteq a \times b$$ la table telle que $$f = (a, b, c)$$. Etant donné un ensemble générique $$x$$, on note $$P$$ la propriété « il existe un ensemble $$y \in b$$ tel que $$(x, y) \in c$$ ». D'après l'axiome de compréhension, il existe un unique ensemble $$d \subseteq a$$ tel que pour tout ensemble $$x$$, il y ait équivalence entre les affirmations « $$x \in d$$ » et « $$x \in a \land x$$ vérifie $$P$$ ». Ceci conclut.

### Ensemble image
Soit $$f : a \to b$$. On appelle **ensemble image** de la fonction $$f$$ l'ensemble $$d \subseteq b$$ tel que pour tout $$y \in d$$, il existe $$x \in a$$ tel que $$f(x) = y$$.

**Preuve.** Il faut montrer ici que $$d$$ existe et est un ensemble. Soit $$c \subseteq a \times b$$ la table telle que $$f = (a, b, c)$$. Etant donné un ensemble générique $$y$$, on note $$P$$ la propriété « il existe un ensemble $$x\in a$$ tel que $$(x, y) \in c$$ ». D'après l'axiome de compréhension, il existe un unique ensemble $$d \subseteq b$$ tel que pour tout ensemble $$y$$, il y ait équivalence entre les affirmations « $$y \in d$$ » et « $$y \in b \land y$$ vérifie $$P$$ ». Ceci conclut.
