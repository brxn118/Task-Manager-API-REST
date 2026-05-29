# TaskManager - API REST Java Spring Boot

Projet personnel : application de gestion de tâches avec une API REST.

## Stack
- Java 17
- Spring Boot 3
- H2 (base de données en mémoire, zéro installation)
- Maven

## Structure du projet
```
taskmanager/
├── pom.xml
└── src/main/java/com/example/taskmanager/
    ├── TaskManagerApplication.java
    ├── model/
    │   └── Task.java
    ├── repository/
    │   └── TaskRepository.java
    └── controller/
        └── TaskController.java
```

## Endpoints disponibles
| Méthode | URL            | Description               |
|---------|----------------|---------------------------|
| GET     | /tasks         | Liste toutes les tâches   |
| GET     | /tasks/{id}    | Récupère une tâche par id |
| POST    | /tasks         | Crée une nouvelle tâche   |
| PUT     | /tasks/{id}    | Modifie une tâche         |
| DELETE  | /tasks/{id}    | Supprime une tâche        |

## Lancer le projet
1. Installer Java 17+ et Maven
2. Dans le dossier taskmanager/ : mvn spring-boot:run
3. Tester avec Postman ou curl
