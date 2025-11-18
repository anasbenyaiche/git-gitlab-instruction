
# Exercice Collaboratif Git/GitLab

## Le Livre de Recettes du Groupe -- Travail en équipe et Merge Requests

Objectif : collaborer avec Git et GitLab en créant des branches, des
commits, des Merge Requests, en réalisant des revues de code et en
résolvant des conflits.

------------------------------------------------------------------------

## 1. Phase 1: Préparation

Créer un projet GitLab :\
`livre-recettes-groupe`

Ajouter la structure suivante :

    README.md
    recettes/
      template.md
      exemple_pates.md

Contenu recommandé pour `template.md` :

``` md
# Titre de la recette

- Auteur : <nom>
- Temps : <X min>
- Difficulté : <facile/moyen/difficile>

## Ingrédients
- ingrédient 1
- ingrédient 2

## Étapes
1. étape 1
2. étape 2
```



------------------------------------------------------------------------

## 2. Phase 2: Clone - Opération

### Étape 0 --- Cloner le projet



### Étape 1 --- Créer une branche personnelle

``` bash
feature/<prenom>-recette
```

Exemple :\
`feature/nom-recette`

### Étape 2 --- Créer votre recette

Copier le modèle :

``` bash
cp recettes/template.md recettes/<prenom>_recette.md
```

Éditer le fichier.

Vérifier l'état 

Ajouter le fichier 

``` bash
 recettes/<prenom>_recette.md
```
Commit 


### Étape 3 --- Envoyer la branche vers GitLab



### Étape 4 --- Créer une Merge Request

1.  Aller dans *Merge Requests → New Merge Request*
2.  Choisir la branche personnelle → comparer avec `main`
3.  Titre : "Ajout de la recette de `<prenom>`"
4.  Ajouter une description
5.  Assigner un reviewer
6.  Créer la MR

### Étape 5 --- Revue de code 


-   ouvrir la MR d'un autre membre
-   lire les modifications
-   ajouter au moins deux commentaires
-   proposer une petite amélioration


Le reviewer clôture les discussions puis approuve la MR.

### Étape 6 --- Fusionner la MR

Fusionner dans `main` (merge ou squash).

------------------------------------------------------------------------

## 3. Phase : Gestion des conflits

Modifier :

`recettes/exemple_pates.md`




Puis fusionner la MR.

------------------------------------------------------------------------

## 4. Options supplémentaires

-   organisation via Issues GitLab\
-   labels personnalisés\
-   protection de la branche `main`\
-   obligation d'approbation avant merge\
-   convention de nommage des branches :



------------------------------------------------------------------------
