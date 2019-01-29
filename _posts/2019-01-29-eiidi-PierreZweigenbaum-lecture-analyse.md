---
layout: post
title:  "Lectures comparées / biomédical"
date:   2019-01-29 11:38:36 +0100
categories: eidi projet Pierre Zweigenbaum
---

## Étude comparative de deux publications sur la normalisation de concepts dans le domaine biomédical.

Pierre Zweigenbaum

### Articles

1. Leaman R, Islamaj Dogan R, Lu Z. DNorm: disease name normalization with pairwise learning to rank. Bioinformatics. 2013 Nov 15;29(22):2909-2917. [PDF](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3810844/)

2. Limsopatham N, Collier N. Normalising medical concepts in social media texts by learning semantic representation. In Proceedings of the Association of Computational Linguistics Annual Meeting (ACL 2016), Berlin, Germany, 2016:1014-1023. [PDF](http://www.aclweb.org/anthology/P16-1096})


### Questions
#### Questions analytiques (~ 2 x 1 page)

    Quel est l'objectif principal du travail ?
    Décrire la méthode employée :
        La résumer (maximum cinq lignes).
        Quels composants élémentaires de traitement utilise-t-elle (ex.  : segmenteur en phrases, étiqueteur, etc.) ?
        Quelle représentation est construite pour chaque exemple ?
        Quel type de classifieur est employé ?
        A-t-elle besoin de connaissances spécifiques (lexiques, corpus, etc.) sur le domaine traité ?
    Évaluation :
        Quels jeux de données sont utilisés, pour l'entraînement et pour le test ? Quelle est leur taille en nombre d'exemples ?
        Quelles mesures d'évaluation sont employées ?
        Les résultats obtenus sont-ils meilleurs que ceux des travaux antérieurs ?
        Quels sont les principaux avantages et inconvénients de la méthode proposée ?


#### Questions de réflexion (~ 2 pages)

    Quelles sont les différences entre ces deux articles en termes de méthodes, de données ou de résultats ? (max 1 page)
    Vous avez été recruté(e) pour continuer et améliorer ce travail :
        Qu'essayez vous en premier ? (max 1/2 page)
        Voyez-vous d'autres pistes à explorer ? (max 1/2 page)

Modalités pratiques

Ne pas hésiter à se mettre en binôme.
Format :
    Police Times 12, marges 2,5 cm, simple interligne, en français (anglais possible aussi)



Références BibTeX :

@article{Leaman:BIOINFORMATICS2013,
abstract = {MOTIVATION: Despite
the central role of diseases in biomedical research, there have been
much fewer attempts to automatically determine which diseases are
mentioned in a text-the task of disease name normalization
(DNorm)-compared with other normalization tasks in biomedical text
mining research. METHODS: In this article we introduce the first
machine learning approach for DNorm, using the NCBI disease corpus and
the MEDIC vocabulary, which combines MeSH(R) and OMIM.  Our method is
a high-performing and mathematically principled framework for learning
similarities between mentions and concept names directly from training
data. The technique is based on pairwise learning to rank, which has
not previously been applied to the normalization task but has proven
successful in large optimization problems for information
retrieval. RESULTS: We compare our method with several techniques
based on lexical normalization and matching, MetaMap and Lucene. Our
algorithm achieves 0.782 micro-averaged F-measure and 0.809
macro-averaged F-measure, an increase over the highest performing
baseline method of 0.121 and 0.098, respectively. AVAILABILITY: The
source code for DNorm is available at
http://www.ncbi.nlm.nih.gov/CBBresearch/Lu/Demo/DNorm, along with a
web-based demonstration and links to the NCBI disease corpus. Results
on PubMed abstracts are available in PubTator:
http://www.ncbi.nlm.nih.gov/CBBresearch/Lu/Demo/PubTator .},
 author         = {Leaman, Robert and Islamaj Dogan, Rezarta and Lu, Zhiyong},
  journal        = {Bioinformatics},
  month          = {Nov 15},
  number         = {22},
  pages          = {2909--2917},
  title          = {{DN}orm: disease name normalization with pairwise learning to rank},
  volume         = {29},
  year           = {2013},
  url       = {https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3810844/}
}

@InProceedings{limsopatham-collier:2016:P16-1,
  author    = {Limsopatham, Nut  and  Collier, Nigel},
  title     = {Normalising Medical Concepts in Social Media Texts by Learning Semantic Representation},
  booktitle = {Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)},
  month     = {August},
  year      = {2016},
  address   = {Berlin, Germany},
  publisher = {Association for Computational Linguistics},
  pages     = {1014--1023},
  url       = {http://www.aclweb.org/anthology/P16-1096}
}

