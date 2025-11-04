# TP – Projet collaboratif Git/GitLab : “Team Notes”

## Objectif 

Vous intégrez l’équipe du projet **“Team Notes”**.  
Ce dépôt a pour but de rassembler les bonnes pratiques, les notes techniques et les fiches personnelles de l’équipe.  
Chaque participant·e doit :
- planifier sa contribution via une **issue** ;
- la réaliser sur une **branche dédiée** ;
- soumettre une **Merge Request (MR)** complète ;
- **relire et approuver** la MR d’un autre membre ;
- participer à la **résolution d’un conflit multi-fichiers** ;
- contribuer à la **release finale** du projet (v1.0).

Le projet est hébergé sur **GitLab **, avec la branche `main` protégée.  
Aucune modification directe sur `main` n’est autorisée.

---

## Étapes du TP

### Étape 1 – Prise en main du dépôt
La création d'un seul dépôt GitLab initial :  
- Fichiers : `README`, `notes/` (vide), `CONTRIBUTING`, `CHANGELOG`.  
- Branche `main` protégée.  
- MR obligatoire avec au moins **1 approbation** avant fusion.

Chaque participant·e :
- consulte la structure du projet ;
- vérifie ses droits ;
- s’assure de bien comprendre les règles de contribution.

---

### Étape 2 – Création de son issue
Chaque participant·e crée **une issue** décrivant sa contribution :  
- Titre clair (ex. “Ajout de la fiche Aurélie dans notes/”) ;  
- Description du but, du contenu attendu et des critères de validation ;  
- Attribution à soi-même ;  
- Ajout d’un label approprié : *doc*, *feat*, *fix* ou *chore*.

Cette issue sert de base à la future Merge Request.

---

### Étape 3 – Création de la branche et contribution
Chaque personne crée une **branche personnelle** à partir de `main`, en suivant la convention :
`feature/<prenom>-<sujet>`

Sur cette branche :
- créer ou modifier plusieurs fichiers selon le sujet choisi (par ex. un document personnel, une section du README, et une mise à jour du changelog) ;
- réaliser des **commits atomiques et cohérents** ;
- veiller à conserver un historique clair et structuré.

Le formateur vérifie que chaque branche est correctement créée et isolée.

---

### Étape 4 – Publication et Merge Request
Chaque participant·e publie sa branche et ouvre une **Merge Request** vers `main`.  
Le **template de MR pour débutants** doit être suivi :

**Structure conseillée de la MR :**
- Contexte / Pourquoi cette contribution ;  
- Ce qui a été modifié ou ajouté ;  
- Comment vérifier le résultat ;  
- Impacts éventuels (documentation, autres fichiers) ;  
- Lien vers l’issue correspondante ;  
- Checklist de vérification :  
  - [ ] Relecture personnelle effectuée  
  - [ ] Orthographe vérifiée  
  - [ ] Conformité aux règles du projet  
  - [ ] Changements cohérents avec les autres fichiers  

La MR est assignée à une autre personne du groupe pour **review** et **approbation**.

---

### Étape 5 – Revue croisée et approbation
Chaque participant·e :
- relit une MR d’un autre membre ;
- rédige **au moins deux commentaires constructifs** (forme, fond, cohérence) ;
- propose si besoin des ajustements ;
- **approuve** la MR une fois les modifications satisfaisantes.

L’auteur·ice intègre les retours (nouveaux commits) et redemande une approbation.  
Une fois validée, la MR est fusionnée dans `main`.

---

### Étape 6 – Conflit multi-fichiers
Le formateur modifie `main` sur plusieurs fichiers déjà touchés par les participant·e·s (ex. README, CHANGELOG, fichier dans `notes/`) afin de créer un **conflit multi-fichiers**.  
Chaque membre doit :
- identifier les conflits ;
- les résoudre en équipe ;
- documenter dans la MR comment la résolution a été décidée.

L’objectif est de comprendre la logique de Git pour la fusion et la coordination des contributions simultanées.

---

### Étape 7 – Release et clôture du projet
Lorsque toutes les MR sont fusionnées :
- compléter le fichier `CHANGELOG` avec les apports de chaque membre ;
- créer un **tag** et une **release v1.0** dans GitLab ;  
- rédiger la release note : une partie **technique** (changements, structure) et une partie **communication** (résumé clair, ton “marketing” interne).

Le formateur valide la cohérence finale et clôture les issues associées.

---

## Livrables attendus
- 1 issue complète par participant·e (titre, description, label, assignation).  
- 1 branche personnelle bien nommée.  
- 1 Merge Request fusionnée, avec au moins 1 approbation.  
- Participation active à une **revue de MR** (commentaires et validation).  
- Gestion collective d’un **conflit multi-fichiers**.  
- **Release v1.0** avec changelog à jour et note de version.  

---


## Résumé du flux attendu
1. Lecture du projet existant.  
2. Création d’une issue.  
3. Création d’une branche personnelle.  
4. Contribution (plusieurs fichiers modifiés).  
5. Ouverture d’une MR complète.  
6. Revue croisée & approbation.  
7. Fusion & gestion du conflit collectif.  
8. Changelog & release v1.0.
