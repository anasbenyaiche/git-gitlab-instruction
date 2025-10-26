# 🧩 Formation GitLab – Exercices pratiques

---

## **Exercice 1 – Créer un projet GitLab**

1. Connecte-toi sur [https://gitlab.com](https://gitlab.com) (ou sur ton instance locale).  
2. Clique sur **“New project” → “Create blank project”**.  
3. Donne un nom au projet :  
   **formation-gitlab-demo**  
4. Choisis la visibilité : **Private**.  
5. Ne coche pas l’option *“Initialize repository with a README”* (on le fera à la main).  
6. Clique sur **Create project**.  
7. Une fois le projet créé, copie l’**URL HTTPS ou SSH** du dépôt.  
8. Garde cette URL : elle servira pour le clonage lors de l’exercice suivant.

---

## **Exercice 2 – Ajouter des collaborateurs et gérer les droits**

1. Ouvre ton projet GitLab.  
2. Dans le menu latéral, clique sur **“Project → Members”**.  
3. Clique sur **“Invite members”**.  
4. Ajoute les utilisateurs suivants avec leurs rôles :  
   - **Maintainer** : accès complet au projet.  
   - **Developer** : peut pousser du code et créer des Merge Requests.  
   - **Reporter** : lecture seule, peut commenter.  
5. Clique sur **“Invite”** pour valider.  
6. Vérifie que les membres apparaissent avec les bons rôles.  
7. Demande au **Developer** de cloner le projet et de tenter un *push*.  
8. Vérifie que le **Reporter** ne peut pas pousser de code.

---

## **Exercice 3 – Créer et protéger la branche principale**

1. Ouvre un terminal et clone ton projet :  
   ```bash
   git clone <URL_du_dépôt>
   cd formation-gitlab-demo
   ```
2. Crée un premier fichier et fais ton premier commit.  
3. Pousse la branche `main` vers le dépôt distant.  
4. Dans GitLab, ouvre **“Settings → Repository → Protected branches”**.  
5. Clique sur **“Protect branch”** et configure :  
   - **Branch name** : `main`  
   - **Allowed to push** : Maintainers only  
   - **Allowed to merge** : Maintainers only  
6. Clique sur **“Protect”** pour enregistrer.  
7. Demande à un Developer de tenter un `git push origin main` : l’action doit être refusée.

---

## **Exercice 4 – Créer une Merge Request (MR)**

1. Depuis ton terminal (en Developer) : crée une branche `feature/ajout-readme` et ajoute une ligne au `README.md`.  
2. Committe et pousse la branche.  
3. Dans GitLab, clique sur **“Create merge request”**.  
4. Vérifie les paramètres :  
   - **Source branch** : `feature/ajout-readme`  
   - **Target branch** : `main`  
5. Donne un titre clair :  
   **feat: ajout d’un message de bienvenue dans le README**  
6. Ajoute une description expliquant la modification.  
7. Assigne la Merge Request à ton Maintainer.  
8. Le Maintainer commente, approuve et clique sur **“Merge”** pour intégrer la modification.

---

## **Exercice 5 – Configurer les approbations et les CODEOWNERS**

1. Ouvre ton projet GitLab.  
2. Va dans **“Settings → General → Merge request approvals”**.  
3. Active **“Require approvals”** et indique `1`.  
4. Coche **“Require approval from Code Owners”**.  
5. Crée un fichier `CODEOWNERS` à la racine du dépôt :
   ```text
   # Code owners
   README.md   @MaintainerUser
   ```
6. Pousse ce fichier dans une nouvelle branche et crée une MR.  
7. Une fois sur `main`, modifie à nouveau `README.md` dans une autre branche.  
8. Crée une nouvelle MR et vérifie que GitLab demande une approbation automatique du Maintainer avant le merge.

---

## **Exercice 6 – Créer un tag et une release**

1. Ouvre ton terminal :  
   ```bash
   git checkout main
   git pull
   git tag -a v1.0.0 -m "Première version stable"
   git push origin v1.0.0
   ```
2. Dans GitLab, ouvre **“Deploy → Releases”**.  
3. Clique sur **“New release”**.  
4. Sélectionne le tag **v1.0.0**.  
5. Ajoute une description claire :  
   **Version 1.0 – Ajout du README initial et première MR fusionnée.**  
6. Clique sur **“Create release”**.  
7. Vérifie que la release est bien visible avec son tag et sa description.

---
