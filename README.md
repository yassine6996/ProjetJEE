# ProjetJEE
# Encadre par Pr YOUSSFI

Ce projet vise à développer une application de gestion de comptes bancaires en utilisant le framework Spring Boot. L'objectif est de permettre aux utilisateurs de gérer facilement leurs comptes, effectuer des opérations de débit et de crédit, ainsi que consulter les informations relatives à leurs comptes. Le projet est structuré en deux composantes principales : la couche DAO (Data Access Object) qui gère l'accès aux données, et la couche service qui gère la logique métier, les objets de transfert de données (DTOs) et les contrôleurs REST (RestController).

+La couche Dao
    -La création des entités JPA qui représentent les classes qui sont persistées dans une base de données relationnelle, et elles permettent de manipuler ces données de manière transparente en utilisant les fonctionnalités de JPA. 
    ![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/ca2a445d-1a71-4cd5-b1a5-8c749e0e346a)

    -Ajouter interfaces AccountOperationRepository, BankAccountRepository et CustomerRepository qui héritent de l'interface           JpaRepository fournie par Spring Data. L'utilisation de l'interface 'JpaRepository' permet de bénéficier des fonctionnalités de base pour l'accès aux données, telles que les opérations CRUD et d'autres opérations courantes. 
   ![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/84fb9932-32c1-41a0-86f8-8a3aecaa7a33)

    -Ajouter les clients en utilisant l'interface BankAccountService 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/7ffdb272-7b3c-4b80-a224-e3182d0e6a33)

-Ajouter les comptes des deux types CurrentBankAccount et SavingBankAccount pour toute la liste des clients 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/99eed7e6-4218-41a0-b914-476cf4856023)

-Le sauvegard
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/39255019-85a2-4c47-8b4b-f6fe2019e2a5)

-Bank Account sur myphpadmin
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/a2448875-dfb3-4afa-9529-0d5b9454884e)

+Test du couche Dao
-Implementation des methodes
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/828dfc42-7163-4937-840f-fce26adaa8ca)

-Pour ajouter des clients, des comptes et des opérations associées en utilisant l'interface BankAccountService, on utilise une implémentation concrète de cette interface, telle que BankAccountServiceImpl. Cette classe permet de créer de nouveaux clients, de créer des comptes pour ces clients, et d'effectuer des opérations telles que les dépôts et les retraits sur les comptes existants. 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/d3f4b5ce-4bd0-493b-b921-0677f6dc6043)


-Créer les deux classes 'BankAccountRestApi' et 'CustomerRestApiController' au niveau du package web; La classe 'BankAccountRestApi' peut fournir des méthodes pour créer de nouveaux comptes, effectuer des dépôts et des retraits, obtenir des informations sur les comptes, etc. Cette classe peut interagir avec l'implémentation de 'BankAccountService' pour exécuter les opérations bancaires correspondantes. La classe 'CustomerRestApiController', quant à elle, peut être utilisée pour la création de nouveaux clients, la récupération des détails des clients, la mise à jour des informations des clients, etc. Cette classe peut également interagir avec l'implémentation de 'BankAccountService' pour effectuer les opérations liées aux clients. 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/36ed5a3f-92a5-44fc-b9a7-57003ca13d44)
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/3b083ff6-36dd-4803-abae-0ee1ef02d018)


-Ajouter la pagination 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/5eab4400-4afd-421f-85af-dad62111200e)

+Angular
-Generer les composants
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/f681df5f-be91-4719-95ee-a5343a6b3395)

-Ajouter une barre de navigation 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/c056d4cf-d4a9-4135-83e0-2d3c81ab3a1e)

-Pour afficher la liste des clients, on doit installer le module HttpClientModule pour intéragir avec la partie Backend et pouvoir charger les données 

![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/d4bb9636-9422-495b-82c8-223881721b00)

-Créer les deux services appelés CustomerService et AccountService pour pouvoir les injecter dans n'importe quel composant 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/16bfbfd5-99d6-4856-8e7f-3ec4dffb4075)

![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/e8dac409-8afb-4a55-af51-f422cac79273)

-Créer des classes sous le paquet models qui représentent le modèle 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/df19ad97-da7a-4e02-89ee-35114f601b81)

-Créer un fomulaire pour la recherche des clients 
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/8b4e79f2-36d6-4afe-a538-f33acb6672f5)

+TEST
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/a472a887-d544-4f8b-86ad-7d7300833f6b)
![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/250258d1-efec-46c0-b909-3d0b3896de22)












