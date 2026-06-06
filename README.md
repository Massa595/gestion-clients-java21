# gestion-clients-java21
Développement d'une API REST de gestion de clients avec Java 21, Spring Boot 3, PostgreSQL et Maven.

# Gestion Clients - API REST (Java 21 / Spring Boot)

## 📌 Description

Ce projet est une API REST simple de gestion de clients, développée avec Java 21 et Spring Boot.

Il permet de manipuler des clients en mémoire via des opérations CRUD :

- Lister les clients
- Récupérer un client par ID
- Ajouter un client

Ce projet a été réalisé dans un objectif d'apprentissage du développement backend Java moderne.

---

## ⚙️ Technologies utilisées

- Java 21
- Spring Boot 3.x
- Spring Web
- Maven
- Git / GitHub

---

## 🏗️ Architecture

Le projet suit une architecture simple en couches : Controller → Service → Model


- **Controller** : expose les endpoints REST
- **Service** : contient la logique métier
- **Model** : représente les données (Client)

---

## 📦 Fonctionnalités

### 📍 GET /clients
Retourne la liste de tous les clients.

### 📍 GET /clients/{id}
Retourne un client par son identifiant.

### 📍 POST /clients
Ajoute un nouveau client.

Exemple de payload :

```json
{
  "id": 3,
  "nom": "DURAND",
  "email": "durand@mail.com"
}

---

## 🚀 Lancer le projet

###  Prérequis
              Java 21+
              Maven

### Commande
./mvnw spring-boot:run
L'application démarre sur : http://localhost:8080

##  🧪 Exemples d'appels API
Récupérer tous les clients : GET /clients
Récupérer un client        : GET /clients/1
Ajouter un client          : POST /clients
                             Content-Type: application/json
                             {
                              "id": 4,
                              "nom": "MARTIN",
                              "email": "martin@mail.com"
                             }

## 📁 Structure du projet

src/main/java/com/Massa/gestion_clients
│
├── controller
│   └── ClientController.java
│
├── service
│   └── ClientService.java
│
├── model
│   └── Client.java
│
└── GestionClientsApplication.java

##  🎯 Objectif pédagogique

Ce projet permet de comprendre :

Le fonctionnement de Spring Boot
La création d’une API REST
Le pattern Controller / Service
La gestion des requêtes HTTP
La sérialisation JSON automatique

##  🔜 Améliorations possibles
Ajout de PostgreSQL (Spring Data JPA)
Validation des données
Gestion des erreurs (404, etc.)
PUT / DELETE (CRUD complet)
Documentation Swagger
Tests unitaires (JUnit / Mockito)

##   👤 Auteur
Projet réalisé dans un contexte d'apprentissage Java backend.
