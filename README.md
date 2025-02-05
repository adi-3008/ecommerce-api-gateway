Project: E-Commerce Microservices Platform
A scalable and distributed e-commerce platform built using a microservices architecture. The platform includes multiple services for order management, product catalog, inventory, and notifications. An API Gateway was designed to handle routing, authentication, and authorization across services, along with resilience mechanisms such as circuit breakers.

Key Features:
Authentication & Authorization: Secured access using Keycloak with PKCE OpenID Connect implementation.
API Gateway: Centralized request routing, security, and circuit breaker functionality.
Event-Driven Architecture: Integrated Kafka for event streaming between services with Avro serialization for efficiency.
Integration Testing: Used RestAssured and WireMock for testing service interactions.
Monitoring & Observability: Set up Grafana Loki, Prometheus, and Tempo for logging, health monitoring, and distributed tracing.
Containerization: Utilized Docker for packaging and deploying services.

Microservices:
Order Service (GitHub Repository)
Handles order creation, management, and status updates. Communicates with inventory and notification services via Kafka.

Product Service (GitHub Repository)
Manages the product catalog, including CRUD operations for product details and pricing information.

Inventory Service (GitHub Repository)
Tracks and manages inventory levels for products, ensuring availability and real-time updates through Kafka events.

Notification Service (GitHub Repository)
Sends notifications to users about order updates, promotions, and low-stock alerts using Kafka for message queuing.
