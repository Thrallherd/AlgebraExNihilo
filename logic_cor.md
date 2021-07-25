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
### Corollaire (raisonnement par l'absurde)
Soit $$P$$ une affirmation dont la véracité n'a pas encore été déterminée, et soit $$Q$$ une affirmation fausse. Si $$\overline{P} \implies Q$$, alors $$P$$ est vraie.

**Preuve.** D'après l'axiome de réfutation, on sait que $$\overline P$$ est fausse, c'est-à-dire que $$P$$ est vraie par l'axiome du tiers exclu.


__________
### Corollaire (associativité des lois)
Si $$P$$, $$Q$$ et $$R$$ sont trois affirmations, on a $$(P \lor Q) \lor R \iff P \lor (Q \lor R)$$ et on préférera écrire plus simplement $$P \lor Q \lor R$$. De même $$(P \land Q) \land R \iff P \land (Q \land R)$$ et on préférera écrire plus simplement $$P \land Q \land R$$.

**Preuve.** En dressant la table des véracités de $$(P \lor Q) \lor R$$ d'une part, et celle de $$P \lor (Q \lor R)$$ d'autre part, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$(P \lor Q) \lor R \iff P \lor (Q \lor R)$$. Le raisonnement est identique pour montrer que $$(P \land Q) \land R \iff P \land (Q \land R)$$.


_____
### Corollaire (commutativité des lois)
Si $$P$$ et $$Q$$ sont deux affirmations, on a $$P \lor Q \iff Q \lor P$$ et $$P \land Q \iff Q \land P$$.

**Preuve.** En dressant la table des véracités de $$P \lor Q$$ d'une part, et celle de $$Q \lor P$$, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$P \lor Q \iff Q \lor P$$. Le raisonnement est identique pour montrer que $$P \land Q \iff Q \land P$$. 


__________
### Corollaire (distribution de la conjonction sur la disjonction)
Si $$P$$, $$Q$$ et $$R$$ sont trois affirmations, on a $$(P \lor Q) \land R \iff (P \land R) \lor (Q \land R)$$

**Preuve.** En dressant la table des véracités de $$(P \lor Q) \land R$$ d'une part, et celle de $$(P \land R) \lor (Q \land R)$$, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$(P \lor Q) \land R \iff (P \land R) \lor (Q \land R)$$.


__________
### Corollaire (négation de la conjonction et de la disjonction)
Si $$P$$ et $$Q$$ sont deux affirmations, on a les deux équivalences $$\overline{P \lor Q} \iff \overline{P} \land \overline{Q}$$ et $$\overline{P \land Q} \iff \overline{P} \lor \overline{Q}$$.

**Preuve.** En dressant la table des véracités de $$\overline{P \lor Q}$$ d'une part, et celle de $$\overline{P} \land \overline{Q}$$, on voit que ce sont les mêmes. D'après l'axiome de dichotomie, on en déduit que $$\overline{P \lor Q} \iff \overline{P} \land \overline{Q}$$. Le raisonnement est identique pour montrer que $$\overline{P \land Q} \iff \overline{P} \lor \overline{Q}$$. 


__________
### Corollaire (reformulation de l'implication)
$$P \implies Q$$ revient à dire que $$Q \lor \overline P$$ est vraie.

**Preuve.** Comme $$P \land \overline Q$$ est fausse, sa négation $$\overline{P \land \overline Q}$$ est vraie. Via le corollaire précédent, on en déduit que $$\overline P \lor \overline{\overline Q}$$ est vraie. Par l'axiome de remplacement et par le corollaire de double négation, on en déduit que $$\overline{P} \lor Q$$ est vraie. Par commutativité, on conclut bien que $$Q \lor \overline P$$ est vraie.


__________
### Corollaire (implications gratuites)
Si $$P$$ et $$Q$$ sont deux affirmations, on a toujours $$P \implies P \lor Q$$ et $$P \land Q \implies P$$.

**Preuve.** $$P \lor Q \lor \overline P$$ est toujours vraie par le corollaire d'associativité puis par l'axiome du tiers exclu, donc $$P \implies P \lor Q$$. De même, $$ P \lor \overline{(P \land Q)}$$ est équivalente à $$P \lor \overline{Q} \lor \overline{P}$$ qui est toujours vraie, donc $$P \land Q \implies P$$.


__________
### Corollaire (équivalences gratuites)
Si $$P$$ est une affirmation, si $$V$$ et $$F$$ sont des affirmations vraie et fausse respectivement, alors on a $$P \iff P \land V$$ et $$P \iff P \lor F$$.

**Preuve.** Pour montrer que $$P \iff P \land V$$, on voit qu'il s'agit en fait de montrer l'équivalence de deux expressions $$A$$ et $$B$$ qui ont été rédigées avec $$P$$ uniquement. Quelle que soit la véracité de $$P$$, on voit que $$A \equiv B$$ donc par application de l'axiome de dichotomie, on conclut que $$P \iff P \land V$$. On montre de la même manière que $$P \iff P \lor F$$.


__________
### Corollaire (déduction)
Si $$P$$ et $$Q$$ sont deux affirmations telles que $$P \implies Q$$ et $$P$$ sont vraies, alors $$Q$$ est vraie.


**Preuve.** Puisque $$P$$ et $$Q \lor \overline P$$ sont vraies, leur conjonction l'est aussi. On a donc $$P \land (Q \lor \overline P)$$ vraie. Par distribution, $$P \land (Q \lor \overline P) \iff (P \land Q) \lor (P \land \overline{P})$$. Comme $$P \land \overline{P}$$ est toujours fausse, on a au final $$P \land (Q \lor \overline P) \iff (P \land Q)$$ et cette dernière expression est donc vraie. De plus, on a toujours $$\overline{Q} \implies \overline{P} \lor \overline{Q}$$ (via les implications gratuites), soit $$\overline{Q} \implies \overline{P \land Q}$$ par négation de la conjonction. Comme $$\overline{P \land Q}$$ est fausse, on conclut par l'absurde que $$Q$$ est vraie.


_____
### Corollaire (proposition contraposée)
Si $$P$$ et $$Q$$ sont deux affirmations telles que $$P \implies Q$$, alors $$\overline{Q} \implies \overline{P}$$.

**Preuve.** Comme $$P \implies Q$$, l'expression $$Q \lor \overline P$$ est vraie. D'après le corollaire de double négation, on a $$Q \iff \overline{\overline{Q}}$$ donc les expressions $$Q \lor \overline P$$ et $$\overline{\overline{Q}} \lor \overline P$$ sont équivalentes par l'axiome de remplacement. Avec le corollaire de commutativité, on a donc $$Q \lor \overline P \iff \overline{P} \lor \overline{\overline{Q}}$$. La deuxième expression signifiant $$\overline{Q} \implies \overline{P}$$, cela conclut.


__________
### Corollaire (disjonction des cas)
Si $$P$$, $$Q$$ et $$R$$ sont trois affirmations telles que $$P \implies R$$ et $$Q \implies R$$, alors $$(P \lor Q) \implies R$$.

**Preuve.** Par hypothèse, $$P \land \overline R$$ et $$Q \land \overline R$$ sont fausses, donc leur disjonction $$(P \land \overline R) \lor (Q \land \overline R)$$ l'est aussi. Comme $$(P \land \overline R) \lor (Q \land \overline R)$ \iff (P \lor Q) \land \overline R$$, on en déduit que $$(P \lor Q) \land \overline R$$ est fausse, c'est-à-dire bien que $$(P \lor Q) \implies R$$.


__________
### Corollaire (enrichissement d'implication)
Si $$P$$, $$Q$$ et $$R$$ sont trois affirmations, alors l'implication $$(P \implies Q)$$ implique l'implication $$((P \lor R) \implies (Q \lor R))$$.

**Preuve.**
