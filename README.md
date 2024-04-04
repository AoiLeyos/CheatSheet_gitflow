# A propos de Git-Flow

   pour un merge branche au lieu de :

   - `git checkout develop`

   - `git merge feature/header`

   - `git branch -D feature/header`
   
   Il suffit juste d'entrer : 

   - `git flow feature finish header` : il fait le merge automatiquement dans la branche develop

## Commande de base

**Setup & init du dossier :**

   - `git flow init` : Initialise un dossier .git vide, dans le dépôt courant et déplace l'utilisateur sur la branche develop

**Branche**

   - `git flow feature start [branche]` : Crée une branche de feature et en fait la branche courante

   - `git flow feature finish [branche]` : Fusionne la branche de feature sur la branche develop, et supprime la branche feature 

   - `git flow hotfix start [branche]` : Crée une branche de déboggage et en fait la branche courante

   - `git flow hotfix finish [branche]` : Fusionne la branche hotfix à la branche main et dévelop, et supprime la branche hotfix

   - `git flow release start [numero_de_version]` : Crée une nouvelle branche de release à partir de la branche develop

   - `git flow release finish [numero_de_verion]` : Fusionne la branche release sur la branche main et supprime la branche release


**Partage de branche**

   - `git flow feature publish [branche]` : Pousse la branche feature sur le dépôt distant

   - `git flow feature pull [remote] [branche]` : Récupère une branche d'un dépôt distant