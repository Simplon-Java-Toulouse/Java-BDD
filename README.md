Bases de données & Java
===

**LUNDI :**
veille sur les SGBD

Retour sur les corrections des exercices précédents + introduction du mécanisme d'Exception

Install mariadb + prise en main sous ubuntu + Executer le script Shop.sql 
11.1 Afficher les tables de la base de donnée Shop
11.2 Trouver un moyen de décrire une table
11.3 Afficher la table des utilisateurs
11.4 Ajouter à celle-ci votre nom + login uniquement, que remarquez vous sur l'idUser ?
11.5 Afficher-la, si votre nom, n'apparait pas, il faut revenir à l'étape précédente
11.6 Remplacer votre password et afficher la table pour vérifier si vos modifications ont été prises en compte
11.7 Supprimer un utilisateur de votre table et afficher la table pour vérifier si c'est bon
11.8 Regarder bien la description de la table, Supprimer la puis crée la à l'identique
11.9 Dans la table des articles, selectionner les articles dont le prix est supérieur à 100
11.10 Selectionner les articles dont le prix est compris entre 50 et 150 
12.11 Afficher les articles dans l'ordre croissant des prix
12.12 Afficher uniquement la description des articles
12.13 Afficher à l'aide d'une jointure, les utilisateurs qui sont administrateurs
12.14 Afficher les utilisateurs qui sont administrateurs et dont le login est Anderson

Note : toutes les requetes doivent être testé et repertorié dans un fichier à valider avec vos formateurs

**MARDI :**
veille sur le langage SQL + règles des clés primaires et étrangères

En ligne de commande uniquement :

13.1 créer une nouvelle base de donné "Bank"

13.2 créer 2 tables, une pour les clients(CodeCli,nom,prénom) et une pour les comptes(NumCpte,solde,CodeCli);

13.3 ajouter des clients et des comptes associés sachant qu'un client peut avoir plusieurs comptes

13.4 afficher tous les comptes d'une personne

13.5 une fois toutes vos requetes réalisées avec succès, supprimer la base Bank

Note : toutes les requetes doivent être testé et repertorié dans un fichier à valider avec vos formateurs

**MERCREDI :**
veille sur JDBC

back to Eclipse 
Créer un projet Shop + ajouter les drivers mariadb(.jar) après les avoir télécharger dans un repertoire lib que vous aurez ajouter + l'ajouter au build path

Dans une classe TestShop par exemple, après avoir initialiser tous les éléments indispensables à votre connection vers votre base Shop, réalisez les requetes suivantes :

14.1 Ajouter à la table des utilisateurs une nouvelle occurence puis afficher la sur votre terminal pour vérification

14.2 Remplacer votre password et vérifier sur votre terminal si c'est bon

14.3 Supprimer un utilisateur de votre table et vérifier

14.4 Afficher toutes les occurences de la table des utilisateurs

14.5 Ajouter une classe Article à votre programme qui correspond à votre table T_Articles puis dans votre prog de test, ajouter une liste d'articles qui contiendra tous les articles que vous pourrez afficher via cette liste.

**JEUDI :**
Veille sur la Gestion des fichiers avec Java 
& les Design pattern

kata : Réaliser le projet Bank, cette fois ci sous Eclipse et en partant de rien !

Révisions

15.1 Maintenant que votre base est crée, Créer le package co.simplon.dao dans lequel vous continuerez vos travaux

15.2 Utiliser un fichier de configuration pour pouvoir changer de SGBD sans devoir toucher votre code

15.3 Utiliser le pattern Singleton afin de vous assurer qu'une seule connection à votre base est ouverte

15.4 Utiliser le pattern DAO(voir d'abord ce qu'est la généricité) pour réaliser les classes ClientDao et CompteDao avec les methodes find(CodeCli) qui renvoi un objet Client grâce à son CodeCli, create(Client) qui insert un client dans sa table, update(Client) qui met à jour un client et delete(Client) qui supprime un client.

15.5 Réaliser une classe TestDao contenant un main pour vérifier toutes les fonctionnalités de vos composants.

15.6 Comment gérer les différents risques telles qu'une création d'un client qui existe déjà ? des requetes malveillantes ? ...

**VENDREDI :**
Veille sur les attaques par injection sql

16.1 Reprener votre projet Bank et trouver un moyen d'éviter les attaques par injection Sql

16.2 Trouver un moyen pour visualiser vos bases de données sous Eclipse

16.3 Bonus : Réaliser un programme permettant de visualiser le contenu de vos lecteurs (fichiers et répertoires)

finir tous les TP et envoyer sur github au plutard dimanche soir

opquast + travailler cv/lm + stage/alternance + atelier communication orale et écrite

Ressources :

[Downloads - MariaDB](https://downloads.mariadb.org)

[Cours et Tutoriels sur le Langage SQL](https://sql.sh/)

[Clés primaires et étrangères - Administrez vos bases de données avec MySQL - OpenClassrooms](https://openclassrooms.com/en/courses/1959476-administrez-vos-bases-de-donnees-avec-mysql/1963057-cles-primaires-et-etrangeres)

[JDBC 4.0 Introduction](https://www.tutorialspoint.com/jdbc/jdbc-introduction.htm)

[KooR.fr - Un ensemble de ressources pédagogiques sur l'API JDBC](http://koor.fr/Java/JDBC.wp)
