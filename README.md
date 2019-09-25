# Pierre Feuille Ciseaux

## Participants

Classe 2020 SIGL - NLPF
 
## Voici les IA déjà mis en place

* Chaque étudiant devra développer sur son IA et sur son dépôt.
* Les dépôts ont été référencés dans le fichier fourni
* Les classes PHP pour les IA ont été nommé de la manière suivante NomdefamillePlayer.php
* Elles se situent dans src/Game/PlayerIA


## Introduction

Vous êtes enfermés avec une autre IA, dont vous ne connaissez pas l'identité.

Vous avez trois choix : pierre (rock), feuille (paper) ou ciseaux (scissors).
En fonction de vos deux choix, les gains (ou pertes) sont répartis de la manière suivante.

| Moi @ L'autre | pierre          | feuille    | ciseaux   |
| ------------- | --------------- | ---------- |---------- |
| pierre        | 1 @ 1           | 0 @ 5      | 5 @ 0     |
| feuille       | 5 @ 0           | 1 @ 1      | 0 @ 5     |
| ciseaux       | 0 @ 5           | 5 @ 0      | 1 @ 1     |

## Comment faire ?

A chaque tour, vous devez faire un choix 'rock', 'paper' ou 'scissors', en fonction du contexte.

## Objectif

Il faut avoir le plus haut score. Les scores se cumulent entre chaque match.

## Informations

Il y a un nombre défini de tours par match.
Pour vous aidez à faire vos choix, vous avez accès aux informations suivantes :
- votre (ou son) dernier choix
- la pile de vos (ou ses) choix
- votre (ou son) dernier gain (ou perte)
- la pile de vos (et ses) gains (ou pertes)
- des statistiques (pour vous, pour l'autre ou les deux) concernant le nombre de fois : où il a été dit 'rock', 'paper', 'scissors'' et le score de chacun
- le numéro du tour où vous en êtes (le tour 0 signifie le premier tour)

Les informations sont dans la proprieté result de votre objet.

## Les scripts à connaitre

./phpunit.phar : permet de lancer les tests (ils seront lancés AVANT de lancer tous les combats)
php EntryPoint.php : permet de lancer les combats ET de générer un fichier index.html avec l'ensemble des résultats

## Les résultats - Etape par Etape

* Récupération de vos classes que je remplace
* Remplacement (ou non) de la classe Crazy par les autres IA
* Execution des tests qui permettent de vérifier s'il n'y a pas eu triche et que vos IAs sont compatibles (si une IA ne passe pas les tests ==> c'est la disqualification)
* Generation de la page de résultats

## Notes

- Les boucles infinis, l'utilisation de die, exit, exceptions, signal, ... sont interdits.
- Une vérification du temps d'execution sera effectué.
- Les valeurs de la matrice de gains/pertes sont amenées à évoluer, ainsi que le nombre de tours pour un match (le nombre de tours sera toujours supérieur à 100).


## Quotes

Prediction is very difficult, especially about the future.
-Niels Bohr
