---
layout: post
title:  "projet EIDI - compréhension (NLU)"
date:   2017-12-28 11:38:36 +0100
categories: eidi projet
---

* Table des matières
{:toc}

## Description générale
{:.no_toc}
Le projet porte sur le développement d'un système de compréhension et surtout l'évaluation et l'analyse des résultats. Le corpus d'apprentissage (trn) fourni contient essentiellement des données artificielles. La question à laquelle il faudra répondre est : quel est l'impact de données artificielle sur la qualité finale ?

Le projet pourra se faire individuellement ou en binôme, mais dans le cas d’un binôme, le rapport devra très clairement indiquer l’apport de chaque membre du binôme et dans ce cas une comparaison entre méthode est attendue (voir Section Sujet).

### Introduction

Les approches fondées sur de l'apprentissage supervisé nécessitent de grandes quantités annotés. Celles-ci sont coûteuses à obtenir. La question qu'on se pose ici est la suivante : peut-on utiliser des données artificiellement générées ?

### Sujet

À partir des données d'apprentissage fournies, il conviendra d'apprendre un modèle supervisé. Vous devez choisir l'approche (*réseaux de neurones* ou *crf*). Les données sont artificielles, c'est à dire qu'elles sont générées à partir de listes de concepts et de patrons simples.

L'objectif est d'évaluer et analyser les résultats obtenus : est-ce que des données artificielles permettent d'apprendre efficacement un système ? Quels sont les limites ? Les erreurs les plus fréquentes ? quelles sont les forces et faiblesses de l'approche choisie étant donné le problème posé au départ (pas de données d'apprentissage autre que les données artificielles). Les différentes classes de données doivent vous guider dans votre analyse.
Enfin une petite analyse des limites de cet analyse est attendue.

### Données

Le domaine est la cuisine. Le système de compréhension porte sur la recherche de recette avec ou sans ingrédients ou famille d'ingrédients spécifiques.

Le corpus dans son ensemble a été constitué à partir de patron de questions et de lexiques tirés de différents sites (wikipdia et marmiton.org). Il a été constitué entièrement automatiquement. Il s'agit donc d'un corpus artificiel.

De façon classique, trois sous-corpus à partir de l'ensemble complet des données ont été constitués, apprentissage (trn), développement (dev), et évaluation (test).

Dans un premier temps, les lexiques ont été subdivisés en lexique de trn, dev et test. Les patrons ont subit le même découpage. Dans chaque cas, une répartition 70/15/15 a été suivie en donnant l'avantage aux données de test sur les données de dev. Quelques patrons différents, plus complexes, ont été réservés pour le test.

Les données de trn ont été générés automatiquement à partir des données patrons+lexiques trn. Elles sont disponibles dans cette [archive](https://sophierosset.github.io/docs/generation-projet-trn.tar.gz).

Les données de dev comportent des énoncés nouveaux générées soit à partir de patrons et de listes nouvelles, soit à partir de patrons issus du trn et de listes nouvelles soit à partir de listes du trn et de patrons nouveaux. Elles sont disponibles dans cette [archive](https://sophierosset.github.io/docs/generation-projet-dev.tar.gz).

Les données de test suivent le même schéma auquel on a ajouté des patrons entièrement nouveaux. *Nous discuterons lors de la séance du 16 janvier de quand vous voulez y avoir accès*

Ce découpage a pour objectif de faciliter l'analyse et de la systématiser.

### Règles du jeu

Le système est développé avec les données trn éventuellement augmentées ou diminuées.

Le système est ensuite tuné (les paramètres sont adaptés) sur les données de dev.

Les données de test ne servent qu'à l'évaluation et à l'analyse.

### Rendu

#### Documents
Vous devez rendre dans une seule archive nommée **NOM1(_NOM2)_projet-eidi-slu.tar.gz**


* un rapport format PDF
* le code, un readme et les données supplémentaires le cas échéant

Envoi à **rosset[arobase]limsi[point]fr** au plus tard mardi **6 février**

#### Présentation

* Mardi 13 février

## Pointeurs

- Outils et programmes
    - Pour des CRF ou maxent ou ... utilisez la boîte à outil [WAPITI](https://wapiti.limsi.fr/)
    - Pour des réseaux de neurones, n'importe quelle implémentation existante pour la détection d'entités nommées est utilisables, par exemple [bi-LSTM, issu de Athavale et al. 2016](https://github.com/monikkinom/ner-lstm) ou encore [LSTM+CRF](https://github.com/guillaumegenthial/sequence_tagging)
    - pour évaluer, vous pouvez utiliser [ne-scoring-gen](https://sophierosset.github.io/docs/eval-nlu.tar.gz)
