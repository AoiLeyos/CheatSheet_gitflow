# A propos de Git-Flow

   pour un merge branche au lieu de :

   - `git checkout develop`

   - `git merge feature/header`

   - `git branch -D feature/header`
   
   Il suffit juste d'entrer : 

   - `git flow feature finish header` : il fait le merge automatiquement dans la branche develop

## Commande de base

**Setup & init du dossier :**

   - `git flow init` : Initialise 

**Branche**

   - `git flow feature start [branche]` :

   - `git flow feature finish [branche]` : 

   - `git flow hotfix finish [branche]` :

   - `git flow release start [numero_de_version]` :

   - `git flow release finish [numero_de_verion]` :


**Partage de branche**

   - `git flow feature publish [branche]` :

   - `git flow feature pull [remote] [branche]` :