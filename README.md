# Mon Projet

## Description
Ce projet consiste à développer une application permettant de gérer des comptes bancaires. Chaque compte appartient à un client et peut subir plusieurs opérations de type DEBIT ou CREDIT. Il existe deux types de comptes : les Comptes Courants et les Comptes Épargne.
********************************************************************************************************
# Gestion des Comptes Bancaires

## Description du projet
Ce projet consiste à développer une application permettant de gérer des comptes bancaires. Chaque compte appartient à un client et peut subir plusieurs opérations de type DEBIT ou CREDIT. Il existe deux types de comptes : les Comptes Courants et les Comptes Épargne.

L'application sera développée en utilisant le framework Spring Boot pour la partie back-end et Angular pour la partie front-end.

## Partie 1 : Couche DAO
Cette partie concerne la création de la couche d'accès aux données (DAO - Data Access Object).

### Étapes à suivre :
1. Créer un projet Spring Boot en utilisant les dépendances nécessaires.
2. Définir les entités JPA suivantes :
   - Customer : représente un client et contient les informations relatives à ce dernier.
   - BankAccount : représente un compte bancaire général et contient les informations communes à tous les types de comptes.
   - SavingAccount : représente un compte épargne et hérite de BankAccount.
   - CurrentAccount : représente un compte courant et hérite de BankAccount.
   - AccountOperation : représente une opération effectuée sur un compte bancaire.
3. Créer les interfaces JPA Repository basées sur Spring Data pour chaque entité. Ces interfaces fourniront les méthodes nécessaires pour interagir avec la base de données.
4. Tester la couche DAO en utilisant des cas de test unitaires pour vérifier le bon fonctionnement des opérations CRUD (Create, Read, Update, Delete) sur les entités.

## Partie 2 : Couche Service, DTOs et RestController
Cette partie concerne la création de la couche service qui gère la logique métier, ainsi que l'utilisation de DTOs et la création de RestControllers pour fournir une API REST.

### Étapes à suivre :
1. Créer les classes de services qui implémentent la logique métier pour chaque entité (Customer, BankAccount, SavingAccount, CurrentAccount, AccountOperation).
2. Utiliser des DTOs pour transférer les données entre la couche service et la couche présentation (RestControllers). Créer les classes DTO appropriées pour chaque entité.
3. Créer les RestControllers qui exposent les différentes fonctionnalités de l'application en utilisant les annotations fournies par Spring MVC.
4. Tester les RestControllers en utilisant des outils comme Postman pour vérifier le bon fonctionnement de l'API REST.

## Partie 3 : Couche Front-end avec Angular
Cette partie concerne la création de l'interface utilisateur à l'aide du framework Angular.

### Étapes à suivre :
1. Créez un nouveau projet Angular en utilisant la commande suivante : `ng new nom-du-projet`
2. Définissez les composants Angular nécessaires pour les fonctionnalités du système (liste des clients, détails du compte, opérations bancaires, etc.).
3. Utilisez des services Angular pour communiquer avec l'API REST du backend et effectuer les opérations CRUD sur les comptes bancaires.
4. Concevez les templates HTML et utilisez les directives et les liaisons de données pour afficher les informations et interagir avec l'utilisateur.
5. Testez l'application front-end en exécutant `ng serve` et accédez à l'application via le navigateur

**********************************************************************************************************

L'application sera développée en utilisant le framework Spring Boot et suivra une architecture en couches comprenant une couche DAO, une couche service, des DTOs (Data Transfer Objects) et des RestControllers.
## Installation
1. Clonez le dépôt du projet : `git clone https://github.com/MarshelD/E_Bank`
2. Accédez au dossier backend : `cd backend`
3. Importez le projet backend dans votre IDE préféré (par exemple, Eclipse ou IntelliJ)
4. Exécutez le projet backend en cliquant sur le bouton "Run" de votre IDE

> Note: Assurez-vous d'avoir configuré correctement votre environnement Java et Maven pour exécuter un projet Spring Boot.

5. Accédez au dossier frontend : `cd ../frontend`
6. Installez les dépendances : `npm install`
7. Lancez l'application frontend : `npm start`

> Note: Assurez-vous d'avoir Node.js et Angular CLI installés sur votre machine pour exécuter l'application frontend.

## Structure du Projet
Le projet est divisé en deux parties : le backend développé avec Spring Boot et le frontend développé avec Angular. Cette architecture permet une séparation claire des responsabilités et favorise la scalabilité et la maintenabilité de l'application.



## Contributions
Les contributions sont les bienvenues ! Si vous souhaitez contribuer à ce projet, veuillez consulter le fichier CONTRIBUTING.md pour obtenir des instructions détaillées. Nous apprécions tous les types de contributions, qu'il s'agisse de corrections de bugs, d'améliorations de fonctionnalités ou de suggestions d'amélioration de l'expérience utilisateur.


Nous espérons que vous apprécierez notre application de gestion de comptes bancaires. N'hésitez pas à nous contacter si vous avez des questions ou des commentaires. Bonne utilisation !
