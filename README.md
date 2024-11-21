# ProjetTP_GitKraken

## Question 1
Barre supérieure
    Permet d’accéder aux actions principales comme ouvrir un projet, créer un nouveau dépôt, ou gérer les paramètre


## Question 2
Ouvrir GitKraken : Lancez l'application GitKraken sur votre ordinateur.

    Nouvel espace de travail : Depuis la page d'accueil, cliquez sur l'icône ‘+’ ou sur File > Init Repo pour créer un nouveau dépôt.

    Choisir l’emplacement : Une fois l’option de création de dépôt sélectionnée, une fenêtre s'ouvre pour spécifier l’emplacement où le dépôt sera créé. Vous pouvez choisir un dossier local ou un emplacement             spécifique sur votre disque.

    Nommer le dépôt : ProjetTP_GitKraken   Dans le champ dédié, entrez un nom pour le dépôt. Cela va créer un dossier avec ce nom, qui contiendra tous les fichiers Git associés.
## Question 3
Les branches permettent de :

    Travailler en parallèle : On peut développer une nouvelle fonctionnalité sans modifier la version principale du code.
    Protéger le code principal : Les branches isolent le code en cours de modification ou de test pour éviter les erreurs dans la version stable.
    Collaborer facilement : Plusieurs personnes peuvent travailler sur différentes fonctionnalités en même temps, sans se gêner.

Créer une branche feature à partir de main avec GitKraken

    Ouvrez GitKraken et assurez-vous d’être sur la branche main.
    Faire Clique droit sur create New Branch 
    Entrez le nom de la nouvelle branche, par exemple feature.
    Validez en cliquant sur Create Branch.


## Question 4
    Assurez-vous d’être sur la branche feature : Dans GitKraken, vérifiez que la branche feature est bien sélectionnée en haut de l’interface.
    Modifier le fichier README.md : Ouvrez le fichier README.md dans votre éditeur de texte préféré, ajoutez une ligne de votre choix, puis enregistrez les modifications.
    Vérifier les changements : Retournez dans GitKraken. Vous verrez que le fichier README.md est listé dans les modifications non commit (non validées).
    Sélectionner les changements : Cliquez sur le fichier README.md dans la liste des modifications pour l’ajouter au commit.
Faire un commit :

    Dans le panneau de droite, entrez un message de commit descriptif, comme “Ajout d’une ligne dans README.md”.
    Cliquez sur Commit changes pour valider les modifications sur la branche feature. 
    
## Question 5
Pousser (ou push) une branche vers le dépôt distant est essentiel car cela permet de :

    Partager le travail avec les autres : Les autres membres de l’équipe peuvent accéder aux modifications, suivre le développement et travailler en parallèle.
    Sauvegarder les modifications : Les changements sont sauvegardés de manière centralisée, ce qui protège contre la perte de données locales.
    Préparer l’intégration : Le code peut être révisé et intégré plus facilement, notamment grâce aux pull requests.

Pousser la branche feature vers le dépôt distant avec GitKraken

    Vérifiez que vous êtes sur la branche feature : Assurez-vous que feature est sélectionnée en haut de l’interface GitKraken.

    Pousser la branche :
        Cliquez sur le bouton Push en haut de la fenêtre.
        GitKraken vous demandera si vous souhaitez pousser la branche feature vers le dépôt distant. Confirmez en cliquant sur Push.

    Vérifiez la réussite de l’opération : GitKraken vous affichera un message de confirmation si le push a bien été effectué.    
## Question 6
Qu’est-ce qu’un conflit Git, et quand survient-il ?

    Un conflit Git survient lorsque deux branches modifient les mêmes lignes d’un fichier ou des fichiers incompatibles       entre elles, rendant impossible la fusion automatique des modifications. Par exemple, si deux personnes modifient         simultanément la même ligne dans un fichier README.md, Git ne sait pas quelle version choisir lors de la fusion. Cela     peut arriver pendant un merge ou un rebase, lorsque Git tente de combiner les branches.
## Question 7 : Résolution de conflits dans GitKraken

    Identifier le conflit : Lorsqu’un conflit survient, GitKraken affiche une notification et marque les fichiers conflictuels en rouge.

    Accéder aux fichiers en conflit : Cliquez sur le fichier en rouge pour ouvrir l’outil de gestion des conflits de GitKraken.

    Analyser les différences : GitKraken affiche trois sections dans l’éditeur :
        Incoming (entrante) : Les changements venant de l’autre branche.
        Resolved (résolu) : La zone où vous choisissez les lignes finales.

    Choisir les changements : Pour chaque section en conflit, vous pouvez :
        Sélectionner la version HEAD,
        Sélectionner la version entrante,
        Combiner manuellement les deux en éditant la zone Résolu.

    Marquer comme résolu : Une fois tous les conflits réglés, cliquez sur Mark as resolved.

    Commit de résolution de conflit : GitKraken vous demandera de faire un commit de merge pour enregistrer la résolution des conflits (voir Question 8 pour plus de détails sur le commit de merge).

    Push vers le dépôt distant : Après avoir fait le commit de résolution de conflit, poussez les changements vers le dépôt distant pour synchroniser la branche.

## Question 8 :

Que signifie le terme “commit de merge” ?

    Un commit de merge est un commit spécial créé lors de la fusion de deux branches. Il capture l’état des deux branches au moment de la fusion, incluant les changements des deux côtés, et indique que ces modifications ont été combinées dans une version finale.

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
