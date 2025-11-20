
# Collaborer avec GitLab

Dans cet exercice, vous allez apprendre à collaborer efficacement à l’aide des fonctionnalités clés de **Git** et **GitLab**.
Vous allez créer et gérer des issues, travailler sur une branche, discuter des modifications, gérer des fichiers ignorés, utiliser le *stash* et effectuer un *rebase* avant la fusion.

---

## Étapes principales

### 1. Créer une issue

Créez une nouvelle issue dans GitLab pour améliorer la description du fichier `README_NOM_DE_EQUIPE.md`.
Ajoutez un titre et une description indiquant les points à compléter.

---

### 2. Gérer les issues avec un board

Accédez au tableau (*Board*) des issues, créez une colonne **In Progress**, 
et déplacez l’issue correspondante dans cette colonne.

---

### 3. Créer une merge request

Créez une nouvelle branche dédiée à la correction du fichier `README_NOM_DE_EQUIPE.md`.
Modifiez le contenu pour qu’il soit plus clair et structuré :

```markdown
# Atelier Git & GitLab
### Equipe 1 : KLM-XCA
#name
#feature  - issues 
Ce projet contient les supports et exercices pratiques utilisés durant la formation **Git & GitLab**.

L’objectif est d’apprendre à versionner, collaborer et gérer un projet à l’aide de Git et de la plateforme GitLab.

## Contenu du projet

* [Flux linéaire (Linear Workflow)](linear-workflow.md)
* [Inspection et exploration de l’historique](inspecting.md)
* [Modification et correction de commits (Amending Commits)](amending.md)
```

```markdown
# Atelier Git & GitLab
### Equipe 2 : equipe_slp
#name
#feature  - issues 
Ce projet contient les supports et exercices pratiques utilisés durant la formation **Git & GitLab**.

L’objectif est d’apprendre à versionner, collaborer et gérer un projet à l’aide de Git et de la plateforme GitLab.
#name
#feature  - issues 
## Contenu du projet

* [Flux linéaire (Linear Workflow)](linear-workflow.md)
* [Inspection et exploration de l’historique](inspecting.md)
* [Modification et correction de commits (Amending Commits)](amending.md)
```

```markdown
# Atelier Git & GitLab
### Equipe 2 : zpc-tmo
Ce projet contient les supports et exercices pratiques utilisés durant la formation **Git & GitLab**.

L’objectif est d’apprendre à versionner, collaborer et gérer un projet à l’aide de Git et de la plateforme GitLab.
#name
#feature  - issues 
## Contenu du projet

* [Flux linéaire (Linear Workflow)](linear-workflow.md)
* [Inspection et exploration de l’historique](inspecting.md)
* [Modification et correction de commits (Amending Commits)](amending.md)
```

Soumettez ensuite une **merge request** liée à l’issue créée.

---

### 4. Discuter et résoudre des commentaires

Commentez une ligne du fichier dans l’onglet **Changes**, puis ajoutez une suggestion d’amélioration.
Appliquez la correction proposée et marquez la discussion comme résolue.

---

### 5. Utiliser le stash

Ajoutez du contenu temporaire dans un fichier, mettez-le de côté avec un *stash*,
puis restaurez-le pour reprendre le travail sans perdre vos modifications.

---

### 6. Gérer les fichiers à ignorer

Créez des dossiers (par exemple `temp` et `logs`) et configurez un fichier `.gitignore`
pour que ces éléments soient exclus du suivi Git.

---

### 7. Corriger un commit avec amend

Si une petite erreur est détectée après un commit, modifiez le dernier commit
afin de corriger son contenu sans créer un nouveau commit.

---

### 8. Faire un rebase avant la fusion

Avant de fusionner la branche, mettez-la à jour avec la branche principale (`main`)
à l’aide d’un *rebase*. Cela permet de garder un historique clair et d’éviter les conflits lors de la fusion.

---

### 9. Fusionner la merge request

Une fois la branche à jour et toutes les discussions résolues, fusionnez la **merge request** dans la branche principale.
Supprimez ensuite la branche de travail devenue inutile.
