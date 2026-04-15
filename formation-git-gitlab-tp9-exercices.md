# Exercice collaboratif GitLab

## Étape 1 : Initialisation du projet

- Créer un projet sur GitLab  
- Ajouter un fichier `index.html`  
- Ajouter une structure de base contenant une zone destinée à accueillir les cartes  

---

## Étape 2 : Création des branches

Chaque équipe crée sa propre branche avec le nom de son équipe :

- dev  
- test  
- maintenance  
- prod  

Chaque équipe pousse sa branche sur le dépôt distant.

---

## Étape 3 : Création des Issues

Chaque équipe doit créer une Issue dans GitLab avec :

- un titre indiquant l’ajout des entreprises  
- une description claire du travail à faire  
- l’assignation des membres de l’équipe  

L’Issue doit être déplacée dans le tableau de bord au fur et à mesure de son avancement (To Do, Doing, Done).

---

## Étape 4 : Développement

Chaque équipe doit :

- ajouter 3 artiste dans le fichier `index.html`
- Chaque équipe devra ajouter des cartes représentant des ar avec :
nom du groupe
description
type de musique
album
image

Toutes les équipes modifient le même fichier.. 
- respecter la même structure de carte.  
- ajouter un minimum de style pour afficher correctement les cartes  

---

## Étape 5 : Commit et Push

Chaque équipe enregistre ses modifications avec des messages clairs, puis envoie son travail sur sa branche.

---

## Étape 6 : Création des Merge Requests

Chaque équipe crée une Merge Request vers la branche `main`.

La Merge Request doit :

- être liée à l’Issue  
- être assignée à une autre équipe pour la review  

---

## Étape 7 : Code Review

Les équipes doivent relire le travail des autres équipes :

- vérifier la qualité du code  
- proposer des améliorations si nécessaire  
- valider ou refuser la Merge Request  

Aucune Merge Request ne doit être acceptée sans validation.

---

## Étape 8 : Gestion des conflits

Lors de la tentative de fusion avec la branche principale, des conflits vont apparaître.

Chaque équipe doit :

- récupérer les dernières modifications de la branche `main`  
- identifier les conflits dans le fichier  
- corriger manuellement les conflits  
- valider les corrections  

---

## Étape 9 : Validation et Merge

Le responsable de la branche `main` :

- vérifie la qualité du code  
- s’assure que les règles sont respectées  
- valide les Merge Requests  

Les branches sont ensuite fusionnées dans `main`.

---

## Étape finale : Rebase

Une fois plusieurs fusions réalisées, chaque équipe doit mettre à jour sa branche avec la branche principale en utilisant le rebase.
