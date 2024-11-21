# ProjetTP_GitKraken

## Question 1
### Décrivez l’interface de GitKraken et indiquez le rôle de chaque section principale :

Barre supérieure :
  -  Ouvrir un projet.
  - Créer un nouveau dépôt.
  - Accéder aux paramètres et configurations globales.

Panneau de gauche :
- Affiche :
  - Les branches locales et distantes.
  - Les remotes (dépôts distants).
- Actions possibles :
  - Créer ou supprimer une branche.
  - Basculer entre différentes branches.

Panneau central :
  - L’historique des modifications.
  - Les relations entre les branches et les commits.

Panneau de droite :
- Liste les fichiers modifiés :
  - **Unstaged Files** : fichiers non ajoutés.
  - **Staged Files** : fichiers prêts à être validés.
- Sert à :
  - Ajouter un message de commit.
  - Valider les changements avec **Commit Changes**.

Barre inférieure :
- Affiche :
  - La branche active.
  - L’état du dépôt (synchronisé ou non).
- Options disponibles :
  - **Pull** pour récupérer les mises à jour distantes.
  - **Push** pour envoyer vos modifications au dépôt distant.

## Question 2
1. **Ouvrir GitKraken**  
   - Cliquez sur **“+”** ou allez dans **File > Init Repo**.

2. **Choisir l’emplacement**  
   - Sélectionnez un emplacement pour le dépôt :  
     - **Nouveau dossier** : créez un nouveau dossier.  

3. **Nommer le dépôt**  
   - Entrez un nom, par exemple : `ProjetTP_GitKraken`.

4. **Initialisez le fichier demandé**    
   - **Ajouter un `README`** : pour décrire le projet.

5. **Finaliser**  
   - Cliquez sur **Init Repository** pour créer le dépôt.


## Question 3
### Les branches permettent de :

Créer des branches dans un projet Git permet de travailler sur différentes tâches en parallèle sans affecter le code principal. Cela permet de protéger la branche     principale, généralement appelée `main` en évitant d’y introduire des erreurs.


## Question 4
Expliquez comment faire un commit avec GitKraken et capturez l'écran de votre commit :

Pour faire un commit avec GitKraken, ouvrez votre dépôt et modifiez vos fichiers. Une fois les changements effectués, allez dans le panneau "Unstaged Files" et cochez les fichiers à      ajouter. Saisissez un message de commit `Ajout d’une ligne dans README.md` dans le champ dédié, puis cliquez sur "Commit Changes" puis push.


    
## Question 5
Pousser (ou push) une branche vers le dépôt distant est essentiel car cela permet de :

Il est important de pousser les branches vers le dépôt distant pour plusieurs raisons : cela permet de sauvegarder vos travaux sur un serveur externe, de partager vos modifications avec d’autres membres de l’équipe et de conserver une version à jour de votre travail accessible de partout. Cela assure également une meilleure gestion des versions et facilite les collaborations en équipe.

Comment faire ?
1. Assurez-vous que feature est sélectionnée en haut de l’interface GitKraken.
2. Pousser la branche :
Cliquez sur le bouton Push en haut de la fenêtre.
GitKraken vous demandera si vous souhaitez pousser la branche feature vers le dépôt distant. Confirmez en cliquant sur Push.


## Question 6
### Qu’est-ce qu’un conflit Git, et quand survient-il ?
Un conflit Git survient lorsque Git ne peut pas automatiquement fusionner deux branches, car les modifications apportées sur ces branches entrent en contradiction.

Cela se produit généralement dans les situations suivantes :
- Modification du même fichier : Si deux personnes modifient la même ligne d'un fichier dans deux branches différentes, Git ne sait pas laquelle des modifications garder lors du merge.
- Modification du même fichier dans des zones proches : Même si les lignes ne sont pas identiques, si elles sont dans la même section du fichier, Git peut avoir des difficultés à déterminer quelle version doit être conservée.
- Suppression d'un fichier dans une branche et modification dans l'autre : Si un fichier est supprimé dans une branche et modifié dans une autre, Git rencontre un conflit lors de la fusion.

## Question 7 : Résolution de conflits dans GitKraken
1. Identifier le conflit : Lorsqu’un conflit survient, GitKraken affiche une notification et marque les fichiers conflictuels en rouge.
2. Accéder aux fichiers en conflit : Cliquez sur le fichier en rouge pour ouvrir l’outil de gestion des conflits de GitKraken.
   
### GitKraken affiche trois sections :
- Ours : les changements de la branche principale (main).
- Theirs : les changements de la branche fusionnée (feature).
- Base : la version initiale avant les modifications.

### Résoudre le conflit : Vous avez trois options :
- Accepter "Ours" : garder les modifications de la branche principale.
- Accepter "Theirs" : garder les modifications de la branche fusionnée.
- Fusionner manuellement : éditer le fichier pour choisir vous-même les modifications à garder.

3. Valider la résolution :  Une fois le conflit résolu, cliquez sur Stage pour préparer le fichier à être commité.
4. Commit et Push :  Entrez un message de commit, puis cliquez sur Commit Changes. Enfin, poussez les modifications vers le dépôt distant en cliquant sur Push.


## Question 8 :
### Que signifie le terme “commit de merge” ?
Le terme "commit de merge" désigne un commit créé automatiquement par Git lorsqu'on fusionne (ou "merge") deux branches. Ce commit marque le point où deux branches distinctes sont combinées en une seule.

Lorsqu'un merge est effectué, Git prend les modifications de deux branches (par exemple, main et feature) et essaie de les intégrer dans une branche de destination (généralement main). Si tout se passe bien, Git crée un commit de merge qui contient les changements combinés des deux branches.


## Question 9 : À quoi sert une Pull Request dans le flux de travail Git ?

Une Pull Request (PR) permet de proposer des modifications dans une branche pour qu’elles soient examinées avant d’être fusionnées dans une autre branche (souvent main). Elle est essentielle dans les projets collaboratifs, car :

    Elle permet de vérifier le code (revue par d’autres développeurs).
    Elle aide à discuter des changements avec des commentaires.
    Elle garantit que le code est testé et approuvé avant d’être fusionné.

Créer une PR dans GitKraken :

    Naviguez dans l’onglet Pull Requests.
    Sélectionnez la branche source (par ex., feature) et la branche cible (par ex., main).
    Ajoutez un titre et une description pour expliquer vos modifications.
    Validez en créant la PR.

## Question 11 : Comment l’interface de GitKraken aide à visualiser les branches et les commits ?

GitKraken affiche les branches et les commits sous forme d’un graphique coloré, facile à comprendre :

    Chaque branche est une ligne colorée, montrant où elle a divergé ou fusionné.
    Les commits sont représentés par des points sur ces lignes, avec des informations comme le message ou l’auteur.
    Les conflits, les merges, et les tags sont clairement visibles.

Avantages :

    On voit tout l’historique en un coup d’œil.
    Les relations entre les branches et les commits sont faciles à comprendre.
    Pas besoin de taper des commandes compliquées.

## Question 12 : À quoi servent les tags, et comment les crée-t-on dans GitKraken ?

    Utilité des tags :
    Les tags marquent des points importants dans un projet, comme une version stable (par ex. v1.0). Ils permettent de       revenir facilement à un état précis du code.

Créer un tag dans GitKraken :

    Cliquez sur le commit que vous voulez taguer.
    Faites un clic droit et choisissez Create Tag.
    Donnez un nom au tag (ex. v1.0) et validez.

Le tag apparaîtra dans le graphique, et vous pouvez le pousser vers le dépôt distant si nécessaire.
