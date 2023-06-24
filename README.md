# ProjetJEE
# Encadre par Pr YOUSSFI

Ce projet vise à développer une application de gestion de comptes bancaires en utilisant le framework Spring Boot. L'objectif est de permettre aux utilisateurs de gérer facilement leurs comptes, effectuer des opérations de débit et de crédit, ainsi que consulter les informations relatives à leurs comptes. Le projet est structuré en deux composantes principales : la couche DAO (Data Access Object) qui gère l'accès aux données, et la couche service qui gère la logique métier, les objets de transfert de données (DTOs) et les contrôleurs REST (RestController).

+La couche Dao
    -La création des entités JPA qui représentent les classes qui sont persistées dans une base de données relationnelle, et           elles permettent de manipuler ces données de manière transparente en utilisant les fonctionnalités de JPA. 
    ![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/ca2a445d-1a71-4cd5-b1a5-8c749e0e346a)

    -Ajouter interfaces AccountOperationRepository, BankAccountRepository et CustomerRepository qui héritent de l'interface           JpaRepository fournie par Spring Data. L'utilisation de l'interface 'JpaRepository' permet de bénéficier des fonctionnalités      de base pour l'accès aux données, telles que les opérations CRUD et d'autres opérations courantes. 
    ![image](https://github.com/yassine6996/ProjetJEE/assets/75941098/7e05a896-2f04-4256-84e6-eb6c510acc55)


