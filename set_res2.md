---
layout: default
title: Construction des entiers naturels et de leur ensemble
language: fr
handle: /set_res3
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

### Entiers naturels
On appelle **entier naturel** l'ensemble vide, ainsi que tout ensemble $$y$$ pouvant s'écrire sous la forme $$y = x \cup \{ x \}$$ où $$x$$ est un entier naturel.

### Représentation des entiers naturels
On utilisera les symboles (chiffres) suivants pour désigner les dix premiers entiers naturels :

| Chiffre | Ensemble | Chiffre | Ensemble |
| :-----: | :------: | :-----: | :------: |
| 0 | $$\varnothing$$ | 5 | $$4 \cup \{ 4 \} = \{ 0, 1, 2, 3, 4 \}$$ |
| 1 | $$0 \cup \{ 0 \} = \{ 0 \}$$ | 6 | $$5 \cup \{ 5 \} = \{ 0, 1, 2, 3, 4, 5 \}$$ |
| 2 | $$1 \cup \{ 1 \} = \{ 0, 1 \}$$ | 7 | $$6 \cup \{ 6 \} = \{ 0, 1, 2, 3, 4, 5, 6 \}$$ |
| 3 | $$2 \cup \{ 2 \} = \{ 0, 1, 2 \}$$ | 8 | $$7 \cup \{ 7 \} = \{ 0, 1, 2, 3, 4, 5, 6, 7 \}$$ |
| 4 | $$3 \cup \{ 3 \} = \{ 0, 1, 2, 3 \}$$ | 9 | $$8 \cup \{ 8 \} = \{ 0, 1, 2, 3, 4, 5, 6, 7, 8 \}$$ |

A partir du symbole d'un entier naturel donné, on obtient le symbole du prochain en permutant le chiffre le plus à droite au chiffre suivant. Si ce chiffre est 9, on le remet à 0 et on itère cette opération avec le deuxième chiffre le plus à droite. Dans le cas particulier où on effectue cette opération sur tous les chiffres du symbole (c'est-à-dire dans le cas particulier où le nombre naturel est désigné par une succession de 9 uniquement), on adjoint le chiffre 1 tout à gauche à la fin du procédé.

### Axiome de l'infini
Il existe un ensemble $$\mathbb{N}$$ contenant tous les entiers naturels, et eux seulement. L’axiome d’extensionnalité montre alors que $$\mathbb{N}$$ est unique.
