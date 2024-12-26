# 🚑 Localisation en temps réel des ambulances et optimisation des itinéraires pour le transport des patients

## Table des matières
1. [Résumé](#résumé)
2. [Technologies utilisées](#technologies-utilisées)
3. [Architecture du système](#architecture-du-système)
4. [Fonctionnalités du logiciel](#fonctionnalités-du-logiciel)
5. [Exigences de compilation et configuration](#exigences-de-compilation-et-configuration)
6. [Installation et configuration](#installation-et-configuration)
7. [Métadonnées du code](#métadonnées-du-code)
8. [Remerciements](#remerciements)

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

### Étape 1 : Cloner le dépôt
```bash
git clone https://github.com/optimiser-itineraires-des-ambulances
cd optimiser-itineraires-des-ambulances
