---
layout: default
title: Axiomes de logique
language: fr
handle: /logic_axm2
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Axiome premier (tiers exclu)
Pour toute affirmation $$P$$, $$P$$ est vraie ou $$\overline P$$ est vraie, donc $$P \lor \overline P$$ est toujours vraie.

### Axiome second (équivalence d'expressions)
Deux expressions $$A$$ et $$B$$ telles que $$A \equiv B$$ quelles que soient les véracités des affirmations avec lesquelles elles ont été rédigées sont équivalentes.

### Axiome second (associativité des lois)
Si $$P$$, $$Q$$ et $$R$$ sont trois affirmations, on a $$(P \lor Q) \lor R \iff P \lor (Q \lor R)$$ et on préférera écrire plus simplement $$P \lor Q \lor R$$. De même $$(P \land Q) \land R \iff P \land (Q \land R)$$ et on préférera écrire plus simplement $$P \land Q \land R$$

### Axiome troisième (commutativité des lois)
Si $$P$$ et $$Q$$ sont deux affirmations, on a $$P \lor Q \iff Q \lor P$$ et $$P \land Q \iff Q \land P$$.

### Axiome quatrième
Si $$P$$ et $$Q$$ sont deux affirmations, on a les deux équivalences $$\overline P \lor Q \iff \overline{P} \land \overline{Q}$$ et $$\overline P \land Q \iff \overline{P} \lor \overline{Q}$$.

### Axiome second
Si _P_ et _Q_ sont deux affirmations, alors $$P \implies (P \lor Q)$$ est vraie. Dit autrement, _P_ implique _P_ ou _Q_.

### Axiome troisième
Si _P_ et _Q_ sont deux affirmations, alors $$(P \lor Q) \implies (Q \lor P)$$ est vraie. Dit autrement, _P_ ou _Q_ implique _Q_ ou _P_. Par symétrie, $$(Q \lor P) \implies (P \lor Q)$$ est vraie aussi et on a en fait l'équivalence $$(P \lor Q) \iff (Q \lor P)$$. 

### Axiome quatrième
Si _P_, _Q_ et _R_ sont trois affirmations, alors nous avons l'implication $$(P \implies Q) \implies ((P \lor R) \implies (Q \lor R))$$. Dit autrement, si _P_ implique _Q_, alors la disjonction _P_ ou _R_ implique la disjonction _Q_ ou _R_.
