# API Transactional

The **API Transactional** is a microservice responsible for processing sales transactions. This API handles user purchases by deducting items from stock and sending a purchase report to another microservice. If any part of the purchase process fails, all actions are rolled back to ensure data consistency. The API communicates with the Stock, Cart, and Reports microservices, and, like the other services, it uses Spring Security for robust authentication and role-based access control. The API is documented with OpenAPI and Swagger, which facilitates easy exploration and testing of endpoints.

## Features

- **Sales Transaction Processing:** Handle user purchases, deduct stock accordingly, and generate a purchase report.
- **Rollback Mechanism:** Automatically revert all actions if any step of the transaction fails, ensuring data consistency.
- **Inter-Microservice Communication:** Integrates with Stock, Cart, and Reports microservices to deliver a complete transactional flow.
- **Authentication and Authorization:** Secure access using Spring Security, with token-based validation and role-based access control.
- **API Documentation:** Interactive OpenAPI documentation integrated with Swagger.
- **Microservices Architecture:** Designed as a scalable microservice for efficient transaction management.
- **Local URL:** [http://localhost:7575](http://localhost:7575)

## Technologies

- Java
- Spring Boot
- Spring Security
- RESTful API
- Microservices Architecture
- OpenAPI / Swagger
- Gradle

## Getting Started

### Prerequisites

- Java 17 or higher
- Gradle
- A compatible SQL Database

## API Endpoints

Access the interactive documentation via Swagger UI:  
**[http://localhost:7575/swagger-ui.html](http://localhost:7575/swagger-ui.html)**  
This interface provides interactive documentation for all available endpoints, making it easy to understand and test the API.

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/EstebanRCarmona/Api-Transactional-emazon.git
