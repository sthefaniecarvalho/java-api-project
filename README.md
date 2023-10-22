# Project Java Api

Criação Java RESTful API

- Project as part of <a href="https://web.dio.me/">DIO</a> Bootcamp FullStack - Java + Angular

## 🛠 Tecnologias
- Java 17
- Spring Boot 3
- Spring Data JPA
- OpenAPI (Swagger)
- Railway

## Class Diagram

```mermaid
classDiagram
    class User {
        - name: String
        - account: Account
        - features: Feature[]
        - card: Card
        - news: News[]
    }

    class Account {
        - number: String
        - agency: String
        - balance: Number
        - limit: Number
    }

    class Feature {
        - icon: String
        - description: String
    }

    class Card {
        - number: String
        - limit: Number
    }

    class News {
        - icon: String
        - description: String
    }

    User "1" --> "1" Account
    User "1" --> "N" Feature
    User "1" --> "1" Card
    User "1" --> "N" News
```
