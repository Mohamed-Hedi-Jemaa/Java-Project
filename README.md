# Gestion de livres dans une bibliothèque (Java SE/MySQL)
L'application permet de faire les actions suivantes: enregistrer tous les livres et tous les abonnés de la bibliothèque dans la base de données; enregistrer les emprunts et les retours de livres par les abonnés; vérifier si un livre demandé est disponible; connaitre quel abonné a pris quel livre.
vous pouvez utiliser directement l'application (GesBiblio.jar) si vous avez le JDK installé sur votre ordinateur.
Pour que l'application fonctionne, vous devez d'abord importer ou créer la base de données "biblio.sql" dans votre SGBD Mysql.

## Voici les interfaces graphiques de l'application :
## Interface graphique d'enregistrement des livres :
Pour enregistrer un livre, il suffit de saisir son identitfiant et son titre et cliquer sur le bouton "Insertion"; 
pour supprimer un enregistrement il faut juste indiquer l'identifiant et cliquer sur le bouton "Supprimer". 

![code1im1](https://user-images.githubusercontent.com/89652407/149229017-a596e17d-2811-4417-bb6a-8e502081df64.png)

## Interface graphique d'enregistrement des abonnés:
L'insertion et la suppréssion se font comme pour les livres. 

![code3im3](https://user-images.githubusercontent.com/89652407/149229503-e6c49368-fb31-40a1-9f22-2446635f92f3.png)

## Interface graphique d'enregistrement des emprunts et retours de livres:
Pour enregistrer un emprunt ou un retour de livre par un abonné, on doit saisir l'identifiant de l'abonné (IdAbonné) et sélectionner le livre qu'il a emprunté ou retourné dans la liste de choix et cliquer le bouton "Valider".
NB: Les listes de choix dans cette application sont réliées aux tables de la base de données, donc leurs contenus varient en fonction des enregistrements ou suppréssions dans les tables.

![code6im6](https://user-images.githubusercontent.com/89652407/149231021-42cf101f-819c-47b3-8677-696847f9cd0e.png)

## Interface graphique des requêtes:

L'interface graphique des requêtes permet de savoir quel abonné a pris quel livre, lorsqu'on choisi le nom d'un abonné dans la liste de choix des noms des abonnées et qu'on clique sur le bouton "Chercher", la liste des livres que cet abonné a emprunté apparait, sinon la liste sera vide quand l'abonné n'a pris aucun livre. 
Si un livre est emprunté, on peut vérifier le nom de celui qui l'a emprunté en choisissant le titre du livre dans la liste de choix des livres et en cliquant sur le bonton "Chercher".
On peut aussi vérifier la disponibilité d'un livre dans cette interface graphique en choisissant le titre du livre dans la liste de choix 
du bas et en cliquant sur le bouton "Vérifier", si le livre est disponible une boite de dialogue affiche "DISPONIBLE" sinon elle affiche "INDISPONIBLE". 

![code5im5](https://user-images.githubusercontent.com/89652407/149229954-9da1c8bd-29d3-4dd9-9d80-eac52ab2e4de.png)

