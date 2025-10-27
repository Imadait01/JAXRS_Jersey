### Projet Banque – API REST JAX-RS (Spring Boot)
## Description

Ce projet est une application Spring Boot exposant une API RESTful pour la gestion des comptes bancaires.
L’API est développée avec JAX-RS (Jersey) pour illustrer l’intégration d’un service REST dans un environnement Spring Boot.

## Architecture du projet
src/
 └── main/
     ├── java/com/example/demo/
     │   ├── config/
     │   │   └── MyConfig.java            
     │   ├── controller/
     │   │   └── CompteRestJaxRSAPI.java  
     │   ├── entities/
     │   │   ├── Compte.java              
     │   │   └── TypeCompte.java          
     │   ├── repositories/
     │   │   └── CompteRepository.java    
     │   └── DemoApplication.java         
     │
     ├── resources/
     │   ├── static/                      
     │   ├── templates/                   
     │   └── application.properties      
     │
     └── test/java/com/example/demo/
         └── DemoApplicationTests.java    


## Technologies utilisées

Spring Boot (version 3+)

JAX-RS / Jersey pour l’API REST

Spring Data JPA

Hibernate

H2 / MySQL (selon configuration)

Lombok pour réduire le code boilerplate

Maven pour la gestion des dépendances

## Lancement de l’application

Cloner le projet

git clone https://github.com/ton-utilisateur/banque-jaxrs.git
cd banque-jaxrs


## Configurer la base de données
Dans src/main/resources/application.properties :

spring.datasource.url=jdbc:h2:mem:banque
spring.h2.console.enabled=true
spring.jpa.hibernate.ddl-auto=update


## Lancer l’application

mvn spring-boot:run

<img width="1914" height="561" alt="TP7" src="https://github.com/user-attachments/assets/751bc715-33fe-40c9-b528-9d1cdd70283d" />

<img width="1896" height="1011" alt="TP7 1" src="https://github.com/user-attachments/assets/efd5b145-9179-4a87-ac9b-70713a13f8bc" />

