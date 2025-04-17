# 🧠 Sistema de Gestión de Órdenes – Microservicios con Spring Boot

Este proyecto es una aplicación distribuida basada en microservicios, desarrollada con Java y Spring Boot. Simula un sistema de e-commerce básico donde los usuarios pueden registrarse, ver productos disponibles y realizar órdenes. El sistema está compuesto por múltiples servicios independientes que se comunican entre sí utilizando tanto REST como mensajería asíncrona (RabbitMQ).

---

## 📌 Descripción General

- Arquitectura basada en microservicios, siguiendo buenas prácticas de separación de responsabilidades.
- Comunicación síncrona entre servicios mediante `RestTemplate`.
- Comunicación asíncrona mediante `RabbitMQ` para manejo de errores y rollback de stock.
- Seguridad implementada con `Spring Security` y `JWT`.
- Descubrimiento de servicios con `Eureka` y enrutamiento mediante `Spring Cloud Gateway`.
- Pruebas unitarias e integración con `JUnit` y `Mockito`.

---

## 🧩 Microservicios

Cada microservicio tiene su propio repositorio:

- 🔐 [`user-service`](https://github.com/TomiB98/MH-MicroService-UserService): Maneja registro, autenticación y validación de usuarios.
- 📦 [`product-service`](https://github.com/TomiB98/MH-MicroService-ProductService): Administración de productos y stock.
- 🧾 [`order-service`](https://github.com/TomiB98/MH-MicroService-OrderService): Creación y gestión de órdenes. Realiza validaciones cruzadas y comunica errores.
- ✉️ [`email-service`](https://github.com/TomiB98/MH-MicroService-EmailService): Envío de notificaciones ante errores en la creación de órdenes.
- 🌐 [`api-gateway`](https://github.com/TomiB98/MH-MicroService-ApiGateway): Entrada principal al sistema, maneja el enrutamiento y la autenticación.
- 📡 [`eureka-server`](https://github.com/TomiB98/MH-MicroService-UserService): Registro y descubrimiento de servicios.

> Reemplazá los enlaces con tus URLs reales de GitHub.

---

## ⚙️ Tecnologías Utilizadas

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
- Docker (solo para desarrollo local)

---

## 🏅 Certificación

Este proyecto fue desarrollado como parte del programa de formación [**Java Immersion – MindHub**](https://www.acreditta.com/credential/71942f70-0313-4930-8b06-4cb18e3d46fd?utm_source=copy&resource_type=badge&resource=71942f70-0313-4930-8b06-4cb18e3d46fd), donde se adquirieron habilidades prácticas en desarrollo backend con Java y arquitectura de microservicios.

---

## ✅ Estado del Proyecto

✔️ Proyecto finalizado como entregable de certificación.  
🛠️ Puede ser extendido con nuevos servicios, manejo de pagos, dashboards, etc.

---

## 📎 Cómo usar este repositorio

Este repositorio actúa como índice general para navegar los distintos microservicios.

---
