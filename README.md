# Gestion de livres dans une bibliothèque Java SE/MySQL
L'application permet de faire les actions suivantes: enregistrer tous les livres et tous les abonnés de la bibliothèque dans la base de données; enregistrer les emprunts et les retours de livres par les abonnés; vérifier si un livre demandé est disponible; connaitre quel abonné a pris quel livre.vous pouvez utiliser directement l'application (GesBiblio.jar) si vous avez le JDK installé sur votre ordinateur.
Pour que l'application fonctionne, vous devez d'abord importer ou créer la base de données "biblio.sql" dans votre SGBD Mysql.

## Voici les interfaces graphiques de l'application :
Interface graphique d'enregistrement des livres :
Pour enregistrer un livre, il suffit de saisir son identitfiant et son titre et cliquer sur le bouton "Insertion"; pour supprimer un enregistrement il faut juste indiquer l'identifiant et cliquer sur le bouton "Supprimer". 

![code2im2](https://user-images.githubusercontent.com/89652407/149222287-329592c3-59e0-4807-be03-56c6460152da.png)

Interface graphique d'enregistrement des abonnés: L'insertion et la suppréssion se font comme pour les livres. 

![code2im2](https://user-images.githubusercontent.com/89652407/149222548-cfd1dc16-f4be-4cca-a76a-18921dc035c5.png)

Interface graphique d'enregistrement des emprunts et retours de livres:
Pour enregistrer un emprunt ou un retour de livre par un abonné, on doit saisir l'identifiant de l'abonné (IdAbonné) et sélectionner le livre qu'il a emprunté ou retourné dans la liste de choix et cliquer le bouton "Valider".
NB: Les listes de choix dans cette application sont réliées aux tables de la base de données, donc leurs contenus varient en fonction des enregistrements ou suppréssions dans les tables. 

![code2im3](https://user-images.githubusercontent.com/89652407/149222602-df946c55-3149-4516-aab8-f046180c7326.png)

## Interface graphique des requêtes:

L'interface graphique des requêtes permet de savoir quel abonné a pris quel livre, lorsqu'on choisi le nom d'un abonné dans la liste de choix des noms des abonnées et qu'on clique sur le bouton "Chercher", la liste des livres que cet abonné a emprunté apparait, sinon la liste sera vide quand l'abonné n'a pris aucun livre. Si un livre est emprunté, on peut vérifier le nom de celui qui l'a emprunté en choisissant le titre du livre dans la liste de choix des livres et en cliquant sur le bonton "Chercher".
On peut aussi vérifier la disponibilité d'un livre dans cette interface graphique en choisissant le titre du livre dans la liste de choix 
du bas et en cliquant sur le bouton "Vérifier", si le livre est disponible une boite de dialogue affiche "DISPONIBLE" sinon elle affiche "INDISPONIBLE". 

![code2im4](https://user-images.githubusercontent.com/89652407/149222761-0b0a9e6c-a105-4d9a-9e45-c3952ba44c86.png)



