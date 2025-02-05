# E-Commerce Microservices Platform

A scalable and distributed e-commerce platform built using a microservices architecture. The platform includes multiple services for order management, product catalog, inventory, and notifications. An **API Gateway** was designed to handle routing, authentication, and authorization across services, along with resilience mechanisms such as circuit breakers.

## Key Features
- **Authentication & Authorization**: Secured access using **Keycloak** with **PKCE OpenID Connect** implementation.  
- **API Gateway**: Centralized request routing, security, and circuit breaker functionality.  
- **Event-Driven Architecture**: Integrated **Kafka** for event streaming between services with **Avro serialization** for efficiency.  
- **Integration Testing**: Used **RestAssured** and **WireMock** for testing service interactions.  
- **Monitoring & Observability**: Set up **Grafana Loki**, **Prometheus**, and **Tempo** for logging, health monitoring, and distributed tracing.  
- **Containerization**: Utilized **Docker** for packaging and deploying services.

---

## Microservices

1. **[Order Service](https://github.com/adi-3008/ecommerce-order-service)**  
   Handles order creation, management, and status updates. Communicates with inventory and notification services via RestClient and Kafka.  

2. **[Product Service](https://github.com/adi-3008/ecommerce-product-service)**  
   Manages the product catalog for product details and pricing information. 

3. **[Inventory Service](https://github.com/adi-3008/ecommerce-inventory-service)**  
   manages inventory levels for products, ensuring availability and real-time updates.  

4. **[Notification Service](https://github.com/adi-3008/ecommerce-notification-service)**  
   Sends notifications to users about order updates.  

---

## API Gateway

The **API Gateway** serves as a centralized entry point for managing, routing, and securing requests to the backend microservices. It handles the following:  
- **Routing**: Directs incoming requests to the appropriate microservice.  
- **Authentication & Authorization**: Integrated with **Keycloak** for secure access.  
- **Resilience**: Implements **circuit breaker functionality** to maintain system stability during service failures.  

---

## Monitoring and Logging
Integrated with **Grafana Loki**, **Prometheus**, and **Tempo** to provide real-time insights into system health, performance metrics, and distributed tracing.  

---

## Deployment
All microservices are containerized using **Docker** for easy deployment and scalability.  

---

Let me know if you want to customize it further! 😊
