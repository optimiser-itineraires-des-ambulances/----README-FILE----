# 🚑 Localisation en temps réel des ambulances et optimisation des itinéraires pour le transport des patients

## Table des matières
1. [Résumé](#résumé)
2. [Technologies utilisées](#technologies-utilisées)
3. [Architecture du système](#architecture-du-système)
4. [Fonctionnalités du logiciel](#fonctionnalités-du-logiciel)
5. [Exigences de compilation et configuration](#exigences-de-compilation-et-configuration)
6. [Installation et configuration](#installation-et-configuration)
7. [Remerciements](#remerciements)

---

## Résumé
Ce projet propose une architecture logicielle basée sur des **microservices** pour gérer la localisation en temps réel des ambulances et l'optimisation des itinéraires pour le transport des patients.  

---

## Technologies utilisées
- 🛠️ **Back-end** : Spring Boot 3  
- 🖥️ **Front-end** : Angular 18  
- 📱 **Mobile** : Flutter  
- 🗃️ **Bases de données** : MongoDB, PostgreSQL  
- 🌀 **Eureka Server** : Découverte des services  
- 🚪 **API Gateway** : Communication inter-microservices  
- 🐳 **Docker** : Conteneurisation  

---

## Architecture du système
L'architecture repose sur une approche **microservices** pour garantir :  
- **Modularité**  
- **Évolutivité**  
- **Maintenabilité**

---

## Fonctionnalités du logiciel
### 🔒 Gestion des utilisateurs :
- Authentification sécurisée
- Gestion des rôles (admin, ambulancier, utilisateur)

### 🚑 Suivi des trajets :
- Localisation GPS
- Cartes interactives

### 🏥 Gestion des hôpitaux :
- Assignation des trajets aux hôpitaux  
- Calcul des itinéraires optimaux  

---

## Exigences de compilation et configuration
- **Langages** : Java 17+, TypeScript  
- **Frameworks** : Spring Boot 3, Angular  
- **Bases de données** : MongoDB, PostgreSQL  
- **Dépendances** : Docker, Node.js  

---

## Installation et configuration

**Your project structure should be like this**
- ambulance-project/
- ├── docker_compose/
- ├── FrontendAngular/
- ├── Gateway-EurekaServer/
- ├── service-ambulance/
- ├── service-hopitaux/
- ├── service-trajets/
- ├── service-utilisateur/
- ├── docker-compose.yml
- └── Flutter_Front/
**Creation des images docker**
- docker build -f Dockerfile -t ambulance_project/service-user-docker .n
- docker build -f Dockerfile -t ambulance_project/service-hopitaux-docker .n
- docker build -f Dockerfile -t ambulance_project/service-trajets-docker .n
- docker build -f Dockerfile -t ambulance_project/service-ambulances-docker .n
- docker build -f Dockerfile -t ambulance_project/gateway-docker .n
- docker build -f Dockerfile -t ambulance_project/eureka-server-docker .n
- docker build -f Dockerfile -t ambulance_project/angular-docker .n
- docker build -f Dockerfile -t ambulance_project/flutter-docker .n
**Docker Compose**
- docker-compose up --build

## Remerciements

Nous remercions chaleureusement toute l'équipe pour les efforts déployés et l'engagement tout au long de ce projet.  
Un grand merci également à notre professeur encadrant pour son accompagnement, ses précieux conseils et son soutien tout au long de cette aventure.  

