# Restaurant Management Platform - Microservices Architecture

## 🍽️ Overview
A comprehensive restaurant management platform built using modern microservices architecture, designed to handle all restaurant operations including user management, menu offerings, order processing, delivery management, complaint handling, and automated notifications.



### Core Components
- **Config Server** (port 8888): Centralized configuration management
- **Eureka Server** (port 8761): Service registry and discovery
- **API Gateway** (port 8081): Unified entry point for all client requests
- **Frontend Angular** (port 4200): Web application for users and administrators

### Microservices
- **User Service** (port 8083): User management and authentication with JWT
- **Menu Service** (port 8084): Restaurant menu management with weather-based recommendations
- **Commande Service** (port 8090): Order processing and management
- **Livraison Service** (port 8085): Delivery management and tracking
- **Reclamation Service** (port 8082): Customer complaint handling
- **Notification Service** (port 8091): Real-time notifications via email

### Infrastructure Services
- **Kafka & Zookeeper** (ports 9092, 2181): Message broker for async communication
- **Prometheus & Grafana** (ports 9090, 3005): Monitoring and visualization
- **Databases**:
  - MongoDB (port 27017): For user and order data
  - MySQL (port 3307): For complaints management
  - PostgreSQL (port 5432): For delivery management
  - H2 Database (port 8092): For menu data

## 🔒 Security
- JWT-based authentication and authorization
- Microservices-specific security configurations
- Secure inter-service communication via Feign clients
- CORS configuration for frontend-backend communication

## 🚀 Features
- **User Management**: Registration, authentication, role-based access control
- **Menu Management**: Dynamic menu with weather-based food recommendations
- **Order Processing**: Secure ordering system with payment integration
- **Delivery Tracking**: Real-time delivery status updates
- **Complaint Handling**: Customer support with status tracking
- **Notifications**: Real-time email alerts for orders, deliveries, and complaints

## 🔧 Technologies
- **Backend**: 
  - Spring Boot, Spring Cloud, Spring Security
  - Node.js (Express) for Notification Service
  - JWT for authentication
  - Feign clients for inter-service communication
  
- **Frontend**: Angular, Bootstrap, RxJS

- **Data Storage**: 
  - MongoDB
  - MySQL
  - PostgreSQL
  - H2 Database

- **DevOps**:
  - Docker & Docker Compose
  - Prometheus & Grafana for monitoring

- **Messaging**:
  - Kafka for asynchronous communication

## 📋 Getting Started

### Prerequisites
- Docker and Docker Compose
- JDK 17+
- Node.js 16+
- Maven



 Access the application:
- Frontend: http://localhost:4200
- API Gateway: http://localhost:8081
- Eureka Dashboard: http://localhost:8761
- Grafana Dashboard: http://localhost:3005 (admin/admin)


## 📊 Monitoring
- Prometheus is configured to scrape metrics from all services
- Grafana dashboards are available for visualizing service performance
- Health endpoints available at `/actuator/health` for each service

## 🔄 API Documentation
- API Gateway routes all requests to appropriate microservices
- Swagger documentation available at `/swagger-ui.html` for each service

## 🤝 Contribution Guidelines
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add some amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a pull request



## 👨‍💻 Created By
Aymen Jallouli


