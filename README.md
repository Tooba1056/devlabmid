Project Name: Database and Cache Services with Docker
Overview
This project sets up two core services within a Dockerized environment:

Database Service: A PostgreSQL database server.
Cache Service: A Redis server used for caching data.
Both services are containerized using Docker and managed through Docker Compose for ease of deployment.

Services
1. Database Service (PostgreSQL)
The PostgreSQL service serves as the database layer for the application, providing persistent storage. It is exposed on port 5432 and uses environment variables to manage sensitive information such as the database user, password, and database name.

2. Cache Service (Redis)
The Redis service is a high-performance caching layer, helping speed up data retrieval processes by caching frequently accessed data. It is exposed on port 6379.

Getting Started
Prerequisites
Ensure you have Docker and Docker Compose installed.

Environment Variables
A .env file is used to store environment variables for configuring the PostgreSQL service, including:

POSTGRES_USER: Specifies the PostgreSQL user.
POSTGRES_PASSWORD: Sets the password for the PostgreSQL user.
POSTGRES_DB: Defines the database name.
To keep sensitive data secure, the .env file is added to .gitignore, preventing it from being committed to version control.
