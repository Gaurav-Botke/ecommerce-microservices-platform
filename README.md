# ecommerce-microservices-platform
A cloud-native distributed backend system built using Spring Boot and Microservices architecture to handle product catalog, order processing, inventory management, and real-time notifications with both synchronous and event-driven communication patterns.

🚀 Scalable E-Commerce Microservices Platform
📌 Overview

This project is a cloud-native microservices-based e-commerce backend system designed to handle product catalog management, order processing, inventory validation, and real-time notifications using modern distributed system design patterns.

🎯 Problem Statement

Traditional monolithic e-commerce systems suffer from scalability issues, tight coupling, and lack of fault tolerance.
This project addresses these challenges by implementing a loosely coupled, scalable, and resilient microservices architecture.

⚙️ Architecture
Product Service – Manages product catalog (MongoDB)
Order Service – Handles order placement
Inventory Service – Checks product availability (MySQL)
Notification Service – Sends order notifications
API Gateway – Entry point for all client requests
🔗 Communication Patterns
Synchronous: OpenFeign (Order → Inventory)
Asynchronous: Apache Kafka (Order → Notification)

🛠️ Tech Stack
Backend: Java, Spring Boot
Microservices: Spring Cloud (OpenFeign, Eureka, Gateway)
Messaging: Apache Kafka
Database: MongoDB, MySQL
Containerization: Docker, Docker Compose
Resilience: Resilience4j
Security: Keycloak
Observability: Prometheus, Grafana, Loki, OpenTelemetry

💡 Key Features
Microservices architecture with independent deployability
Event-driven communication for scalability
Fault tolerance using Circuit Breaker
API Gateway routing and filtering
Service discovery using Eureka
Database per service design pattern

📈 Impact
Improved system scalability and maintainability
Reduced service coupling through async communication
Increased fault tolerance using resilience patterns
Enabled real-time event processing with Kafka
