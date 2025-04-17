# 🧠 Order Management System – Microservices with Spring Boot

This project is a distributed application based on microservices, developed using Java and Spring Boot. It simulates a basic e-commerce system where users can register, browse products, and place orders. Each microservice is responsible for a specific domain and communicates with others via REST or asynchronous messaging using RabbitMQ.

---

## 📌 Overview

- Microservices architecture following best practices and domain separation.
- Synchronous communication via `RestTemplate`.
- Asynchronous messaging with `RabbitMQ` for error handling and stock rollback.
- Security implemented with `Spring Security` and `JWT`.
- Service discovery with `Eureka` and routing via `Spring Cloud Gateway`.
- Unit and integration testing using `JUnit` and `Mockito`.

---

## 🧩 Microservices

Each microservice has its own dedicated repository:

- 🔐 [`user-service`](https://github.com/TomiB98/MH-MicroService-UserService): Handles user registration, authentication, and validation.
- 📦 [`product-service`](https://github.com/TomiB98/MH-MicroService-ProductService): Manages products and stock.
- 🧾 [`order-service`](https://github.com/TomiB98/MH-MicroService-OrderService): Handles order creation, validations, and error messaging.
- ✉️ [`email-service`](https://github.com/TomiB98/MH-MicroService-EmailService): Sends email notifications in case of order failures.
- 🌐 [`api-gateway`](https://github.com/TomiB98/MH-MicroService-ApiGateway): Entry point to the system, handles routing and authentication.
- 📡 [`eureka-server`](https://github.com/TomiB98/MH-MicroService-EurekaServer): Service registry and discovery.

---

## ⚙️ Technologies Used

- Java 
- Spring Boot  
- Spring Web (REST APIs)  
- Spring Security + JWT  
- Spring Cloud Gateway  
- Eureka Server / Client  
- RabbitMQ  
- RestTemplate  
- JUnit & Mockito  
- H2 Database 
- Docker (for local development)

---

## 🏅 Certification

This project was developed as part of the [**Java Immersion – MindHub**](https://www.acreditta.com/credential/71942f70-0313-4930-8b06-4cb18e3d46fd?utm_source=copy&resource_type=badge&resource=71942f70-0313-4930-8b06-4cb18e3d46fd) training program, focused on backend development and microservices architecture with Java.

---

## ✅ Project Status

✔️ Completed as a final certification project.  
🛠️ Easily extendable with features like payment integration, dashboards, etc.

---

## 📎 About this Repository

This repository serves as a central hub linking to each microservice.

---
