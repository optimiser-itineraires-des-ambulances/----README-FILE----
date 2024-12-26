🚑 Localisation en Temps Réel des Ambulances et Optimisation des Itinéraires
Ce projet propose une solution logicielle basée sur des microservices pour suivre la localisation en temps réel des ambulances et optimiser les trajets pour le transport des patients. Il intègre des technologies modernes telles que Spring Boot, Angular, Flutter, MongoDB, et PostgreSQL, avec une architecture robuste et évolutive.

📚 Table des Matières
Résumé
Technologies Utilisées
Architecture du Système
Fonctionnalités du Logiciel
Exigences de Compilation et Configuration
Installation et Configuration
Cloner le Dépôt
Démarrer avec Docker
Métadonnées du Code
Remerciements

✨ Résumé
Ce projet utilise une architecture microservices pour assurer une modularité et une évolutivité maximales. Les principaux composants incluent :

Un front-end Angular pour la gestion des utilisateurs et des trajets.
Un back-end Spring Boot pour la logique métier.
Une application mobile Flutter pour les utilisateurs finaux.
Bases de données MongoDB et PostgreSQL pour la gestion des données.
Eureka Server et API Gateway pour la communication entre microservices.

🛠️ Technologies Utilisées
Microservices (Spring Boot)
Angular 18
Flutter
MongoDB & PostgreSQL
Eureka Server & API Gateway
Docker
Maven

🏗️ Architecture du Système
Vue d'ensemble :
Microservices Back-End : Gestion des utilisateurs, trajets, et ambulances.
Bases de Données : MongoDB (données non relationnelles) & PostgreSQL (données relationnelles).
Eureka Server : Découverte et registre des services.
API Gateway : Point d'entrée unique.
Front-End Angular : Interface administrateur.
Flutter Mobile App : Interface utilisateur.

🚀 Fonctionnalités du Logiciel
Authentification et Gestion des Utilisateurs :
Connexion sécurisée (administrateurs, ambulanciers, utilisateurs).
Gestion des rôles.
Mise à jour des profils.
Gestion des Ambulances et Suivi des Trajets :
Localisation GPS en temps réel.
Suivi des trajets sur une carte interactive.
Gestion des Hôpitaux et Optimisation des Trajets :
Assignation intelligente des trajets.
Calcul d'itinéraires optimaux.
Enregistrement et Affichage des Données :
Tableaux de bord pour les administrateurs.
Historique des trajets sauvegardé en base de données.

⚙️ Exigences de Compilation et Configuration
Java : 17+
Maven : 3.8.1+
Node.js : 16+
Docker : 20.10+
Base de données : MongoDB, PostgreSQL
Frameworks : Spring Boot, Angular, Flutter

🔧 Installation et Configuration
Cloner le Dépôt
bash
Copier le code
git clone https://github.com/votre-repo/ambulance-itineraires
cd ambulance-itineraires
Démarrer avec Docker
Assurez-vous d'avoir Docker installé. Voici les commandes pour démarrer les services.

Créer un fichier docker-compose.yml (déjà inclus dans le dépôt) :
yaml
Copier le code
version: '3.8'
services:
  eureka-server:
    image: eurekaserver:latest
    ports:
      - "8761:8761"

  api-gateway:
    image: apigateway:latest
    ports:
      - "8080:8080"

  backend-service:
    build: ./backend
    ports:
      - "8081:8081"
    depends_on:
      - database

  database:
    image: postgres:latest
    environment:
      POSTGRES_USER: admin
      POSTGRES_PASSWORD: admin
      POSTGRES_DB: ambulance_db
    ports:
      - "5432:5432"
Démarrer les services :
bash
Copier le code
docker-compose up -d
Vérifier l'état :
bash
Copier le code
docker ps

🛡️ Métadonnées du Code
Langage : Java, TypeScript, Dart
Frameworks : Spring Boot, Angular, Flutter
Base de données : PostgreSQL, MongoDB
Conteneurisation : Docker

🙏 Remerciements
Un grand merci à toutes les personnes qui ont contribué à ce projet et à la communauté open source pour leur soutien constant. 🌟

