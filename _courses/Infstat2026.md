---
layout: course
title: Statistique inférentielle
year: 	25/26
semester: S2
hours: 23.5
lang: French
role: CM+TD+TP
nostudents:
level: M1
studtype: Mathematics students of UFR Mathématiques Informatique Mécanique
etab: université de Lorraine
classnumber: 11
#groupnumber : 1
---

<br/>

<a style="color: red; font-weight: bold;">News</a> : [Feuille TD1](https://filesender.renater.fr/?s=download&token=32d916ae-8192-49f9-a3f4-d5f1dec077e8){:target="_blank"}, [Feuille TD2](https://filesender.renater.fr/?s=download&token=3c4ad9fa-30e9-4fcc-b488-efc15ce5fb91){:target="_blank"} <br/>

<!--
#### Consultation des copies du partiel du 15.11.2025

Uniquement sur rendez-vous, s'inscrire via le bouton vert en bas à droite.

<!-- Calendly badge widget begin
<link href="https://assets.calendly.com/assets/external/widget.css" rel="stylesheet">
<script src="https://assets.calendly.com/assets/external/widget.js" type="text/javascript" async></script>
<script type="text/javascript">window.onload = function() { Calendly.initBadgeWidget({ url: 'https://calendly.com/matteopdachille/consultation-des-copies-partiel-15-11-2025', text: 'Consultation des copies du partiel | 2.12.2025 - réservation', color: '#008000', textColor: '#ffffff', branding: false}); }</script>
<!-- Calendly badge widget end
-->
<!--
<br/>
Pour le materiel de cours ainsi que les annonces communs voir : <br/> [#](https://arche.univ-lorraine.fr/course/view.php?id=81800){:target="_blank"}


### Programme (très) synthétique
<!--
1. Vocabulaire élémentaire pour l’étude de fonctions réelles de variable réelle
2. Applications usuelles
3. Primitives usuelles
4. Equations différentielles linéaires

-->


### Textes de référence


+ P-A. Cornillon, N. Hengartner, E. Matzner-Løber, L. Rouvière, _Régression avec R_, edpsciences, [lien](https://regression-avec-r.github.io/){:target="_blank"}
+ A. Guyader, _Statistique mathématique_, notes de cours, Master Mathématiques et Applications, Sorbonne Université, [pdf](https://perso.lpsm.paris/~aguyader/files/teaching/StatMath.pdf){:target="_blank"}
+ A. Monfort, _Cours de statistique mathématique_, Economica, Paris.
+ L. Wasserman, _All of nonparametric statistics_, Springer New York, [lien](https://link.springer.com/book/10.1007/0-387-30623-4
){:target="_blank"}
<br/>

### Tableau de bord

| Leçon n&deg; | Date | Sujet |
|:-: | :---: | :---: |
| 1 | 30.01 | Introduction au modèle de regression linéaire simple. Motivations, définition, hypothèses sur la perturbation. Écriture vectorielle et interpretation géométrique. Méthode d'estimation des moindres carrés ordinaires : forme quadratique des moindres carrés, déduction des estimateurs \\(( \hat{a}, \hat{b})\\), leurs propriétés : centre de gravité, absence de biais, variances et covariance. Théorème de Gauss-Markov (énoncé). Rappels sur la loi normale en dimension 1. |
| 2 | 06.02 | Consequences du Théorème de Gauss-Markov. Coefficient de détermination \\(R^2 \\) et caveat sur son interpretation. Modèle de regression linéaire simple avec perturbation normale. Propriétés des ses estimateurs du maximum de vraisemblance : comparaison avec les estimateurs MCO. Rappel sur les gaussiennes multivariées : méthodes d'échantillonnage, projection orthogonale sur un sous-espace (loi de la norme au carré du projeté), loi jointe des projections orthogonaux sur deux sous-espaces, loi sous l'action d'une matrice symétrique définie positive générale.  Application : loi du triplet \\(( \hat{a}, \hat{b},\hat{\sigma}^2)\\).
| 3 | 13.02 | Prévision dans la regression linéaire simple. Trois exercices sur la regression linéaire simple : calculs de \\(\hat{a}, \hat{b}, R^2\\) (à la main), interpretation géométrique du produit des pentes dans les deux regression possibles. Introduction au modèle de regression multiple : définition et interpretation géométrique. Moindres carrés ordinaires (début).|
| 4 | 20.02 | Propriétés des estimateurs MCO. Théorème de Gauss-Markov (avec démonstration). Application : estimateurs affines sans biais de variance minimale. Coefficient de determination et son interpretation géométrique. Modèle de regression linéaire multiple avec perturbation gaussienne : MCO vs MV, exhaustivité, minimalité et totalité de \\(( \hat{b}^t,\hat{\sigma}^2)\\) et sa loi. Prévision (début).|
| 5 | 06.03 | Prévision (suite), loi de \\(\frac{y-\hat{y}_0}{\sqrt{\sigma^2 \left(1+x^t_0(X^t X)^{-1}x_0 \right)}}\\). Théorème de Frish-Waugh (avec preuve). Rappels d'algèbre linéaire : norme d'un opérateur linéaire, formes quadratiques et integrales gaussiens. Convergence de \\(\hat{b}\\) vers \\(b\\) en moyenne quadratique et p.s. (avec preuve), convergence vers une matrice régulière (avec preuve). Normalité asymptotique de \\(\hat{b}\\) (avec preuve). Convergence en proba de \\(\hat{\sigma}^2\\) vers \\(\sigma^2\\).|
| 6 | 13.03 | [Feuille TD1](https://filesender.renater.fr/?s=download&token=32d916ae-8192-49f9-a3f4-d5f1dec077e8) : Question 1, 2, 3. Exercice 1, interpretation géométrique du niveau de risque de \\(5\\)% comme region autour de la droite de regression|
| 7 | 20.03 | [Feuille TD1](https://filesender.renater.fr/?s=download&token=32d916ae-8192-49f9-a3f4-d5f1dec077e8) : Exercice 2. [Feuille TD2](https://filesender.renater.fr/?s=download&token=3c4ad9fa-30e9-4fcc-b488-efc15ce5fb91) : Question 1, rappels sur la loi de Fisher avec deux exos (+ DM), exercice 1, exercice 2 (début).|
