# My Backend Project

## Overview

This Spring Boot backend project is designed to handle various aspects of an e-commerce system. It comprises several services, including Product Service, Order Service, Notification Service, an API Gateway, and a Eureka Server. These services interact to manage products, process orders, send notifications through Kafka, and are orchestrated with Eureka for service discovery.

## Services

### 1. Product Service

The Product Service is responsible for managing product information. It allows the creation of new products, each defined by a name, price, and available quantity.

### 2. Order Service

The Order Service facilitates the placement of orders. It communicates with the Inventory Service to check product availability and manages the order placement process.

### 3. Inventory Service

The Inventory Service maintains information about product availability. It is consulted by the Order Service to ensure that products are in stock before processing an order.

### 4. Notification Service

The Notification Service uses Kafka to handle notifications. It receives messages from other services, such as the Order Service, to notify users about various events in the system.

### 5. API Gateway

The API Gateway acts as a central entry point for the microservices. It handles routing, composition of microservices, and other cross-cutting concerns.

### 6. Eureka Server

Eureka is a service registry and discovery server. The Eureka Server allows microservices to register themselves and discover other services in the system.

## Technologies Used

The project leverages the following technologies:

- **Spring Boot:** A powerful framework for building Java-based web applications.
- **Docker:** Containerization technology for packaging applications and their dependencies.
- **Kafka:** A distributed streaming platform for building real-time data pipelines and streaming applications.
- **Spring Cloud:** A set of tools and frameworks to build microservices architecture.
- **API Gateway:** Used for routing and composition of microservices.
- **Eureka Server:** A service registry for enabling service discovery.
