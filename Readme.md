### Projet Banque – API REST JAX-RS (Spring Boot)
## Description

Ce projet est une application Spring Boot exposant une API RESTful pour la gestion des comptes bancaires.
L’API est développée avec JAX-RS (Jersey) pour illustrer l’intégration d’un service REST dans un environnement Spring Boot.

## Architecture du projet
src/
└── main/
├── java/com/example/demo/
│   ├── config/
│   │   └── MyConfig.java            # Configuration Jersey (enregistrement des ressources REST)
│   ├── controller/
│   │   └── CompteRestJaxRSAPI.java  # Contrôleur REST (endpoints JAX-RS)
│   ├── entities/
│   │   ├── Compte.java              # Entité représentant un compte bancaire
│   │   └── TypeCompte.java          # Enum pour le type de compte (COURANT, EPARGNE, etc.)
│   ├── repositories/
│   │   └── CompteRepository.java    # Interface JPA pour les opérations CRUD
│   └── DemoApplication.java         # Classe principale (point d’entrée Spring Boot)
│
├── resources/
│   ├── static/                      # Ressources statiques (CSS, JS, images)
│   ├── templates/                   # Templates (si besoin)
│   └── application.properties       # Configuration de l’application
│
└── test/java/com/example/demo/
└── DemoApplicationTests.java    # Tests unitaires de base

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