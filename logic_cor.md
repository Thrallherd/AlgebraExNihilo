---
layout: default
title: Corollaires de logique
language: fr
handle: /logic_cor
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Corollaire (double négation)
Si $$P$$ est une affirmation, alors $$P \iff \overline{\overline P}$$.

**Preuve.** Si $$P$$ est vraie, alors $$\overline P$$ est fausse. Par l'axiome du tiers exclu, on en déduit que la négation de $$\overline P$$ est vraie, c'est-à-dire que $$\overline{\overline P}$$ est vraie. De même si $$P$$ est fausse, on en déduit que $$\overline P$$ est vraie et donc que $$\overline{\overline P}$$ est fausse. Comme $$P$$ et $$\overline{\overline P}$$ ont toujours la même véracité, on conclut par l'axiome de dichotomie que $$P \iff \overline{\overline P}$$.


__________
### Corollaire (associativité des lois)
Si $$P$$, $$Q$$ et $$R$$ sont trois affirmations, on a $$(P \lor Q) \lor R \iff P \lor (Q \lor R)$$ et on préférera écrire plus simplement $$P \lor Q \lor R$$. De même $$(P \land Q) \land R \iff P \land (Q \land R)$$ et on préférera écrire plus simplement $$P \land Q \land R$$.

**Preuve.** En dressant la table des véracités de $$(P \lor Q) \lor R$$ d'une part, et celle de $$P \lor (Q \lor R)$$ d'autre part, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$(P \lor Q) \lor R \iff P \lor (Q \lor R)$$. Le raisonnement est identique pour montrer que $$(P \land Q) \land R \iff P \land (Q \land R)$$. 


_____
### Corollaire (commutativité des lois)
Si $$P$$ et $$Q$$ sont deux affirmations, on a $$P \lor Q \iff Q \lor P$$ et $$P \land Q \iff Q \land P$$.

**Preuve.** En dressant la table des véracités de $$P \lor Q$$ d'une part, et celle de $$Q \lor P$$, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$P \lor Q \iff Q \lor P$$. Le raisonnement est identique pour montrer que $$P \land Q \iff Q \land P$$. 


_____
### Corollaire (proposition contraposée)
Si $$P$$ et $$Q$$ sont deux affirmations telles que $$P \implies Q$$, alors $$\overline{Q} \implies \overline{P}$$.

**Preuve.** Comme $$P \implies Q$$, l'expression $$Q \lor \overline P$$ est vraie. D'après le corollaire de double négation, on a $$Q \iff \overline{\overline{Q}}$$ donc les expressions $$Q \lor \overline P$$ et $$\overline{\overline{Q}} \lor \overline P$$ sont équivalentes par l'axiome de remplacement. Avec le corollaire de commutativité, on a donc $$Q \lor \overline P \iff \overline{P} \lor \overline{\overline{Q}}$$. La deuxième expression signifiant $$\overline{Q} \implies \overline{P}$$, cela conclut.


__________
### Corollaire (distribution de la conjonction sur la disjonction)
Si $$P$$, $$Q$$ et $$R$$ sont trois affirmations, on a $$(P \lor Q) \land R \iff (P \land R) \lor (Q \land R)$$

**Preuve.** En dressant la table des véracités de $$(P \lor Q) \land R$$ d'une part, et celle de $$(P \land R) \lor (Q \land R)$$, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$(P \lor Q) \land R \iff (P \land R) \lor (Q \land R)$$.


__________
### Corollaire (négation de la conjonction et de la disjonction)
Si $$P$$ et $$Q$$ sont deux affirmations, on a les deux équivalences $$\overline{P \lor Q} \iff \overline{P} \land \overline{Q}$$ et $$\overline{P \land Q} \iff \overline{P} \lor \overline{Q}$$.

**Preuve.** En dressant la table des véracités de $$\overline{P \lor Q}$$ d'une part, et celle de $$\overline{P} \land \overline{Q}$$, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$\overline{P \lor Q} \iff \overline{P} \land \overline{Q}$$. Le raisonnement est identique pour montrer que $$\overline{P \land Q} \iff \overline{P} \lor \overline{Q}$$. 


__________
### Axiome second
Si _P_ et _Q_ sont deux affirmations, alors $$P \implies (P \lor Q)$$ est vraie. Dit autrement, _P_ implique _P_ ou _Q_.

### Axiome troisième
Si _P_ et _Q_ sont deux affirmations, alors $$(P \lor Q) \implies (Q \lor P)$$ est vraie. Dit autrement, _P_ ou _Q_ implique _Q_ ou _P_. Par symétrie, $$(Q \lor P) \implies (P \lor Q)$$ est vraie aussi et on a en fait l'équivalence $$(P \lor Q) \iff (Q \lor P)$$. 

### Axiome quatrième
Si _P_, _Q_ et _R_ sont trois affirmations, alors nous avons l'implication $$(P \implies Q) \implies ((P \lor R) \implies (Q \lor R))$$. Dit autrement, si _P_ implique _Q_, alors la disjonction _P_ ou _R_ implique la disjonction _Q_ ou _R_.
