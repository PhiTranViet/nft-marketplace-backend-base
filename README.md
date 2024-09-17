# 🛒 NFT Marketplace Backend

## Overview

This is the backend system for a decentralized NFT Marketplace, designed to handle minting, trading, and managing NFTs. The system is built with a microservices architecture, utilizing technologies like **NestJS**, **Kafka**, **MongoDB**, **Elasticsearch**, and containerized with **Docker**. It provides robust APIs for managing users, assets, and marketplace transactions, ensuring high availability and scalability.

## ✨ Key Features

- **Minting and Trading NFTs**: Create, buy, and sell NFTs on the marketplace.
- **User Management**: Secure user authentication and profile management.
- **Real-time Notifications**: Event-driven architecture with Kafka for real-time notifications.
- **Search and Indexing**: Full-text search capability using Elasticsearch for fast NFT and user searches.
- **Microservices Architecture**: Built with a scalable, maintainable microservices architecture.

## 🛠️ Tech Stack

- **Framework**: [NestJS](https://nestjs.com/)
- **Message Broker**: [Kafka](https://kafka.apache.org/)
- **Database**: [MongoDB](https://www.mongodb.com/)
- **Search Engine**: [Elasticsearch](https://www.elastic.co/elasticsearch/)
- **Containerization**: [Docker](https://www.docker.com/)
- **Container Orchestration**: [Docker Compose](https://docs.docker.com/compose/)

## ⚙️ Setup and Installation

### Prerequisites

Make sure you have installed the following tools:
- **Docker**: [Install Docker](https://docs.docker.com/get-docker/)
- **Docker Compose**: [Install Docker Compose](https://docs.docker.com/compose/install/)

### Step-by-Step Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/phitranviet/nft-marketplace-backend-base.git
   cd nft-marketplace-backend
   ```

2. **Environment Configuration**:
Duplicate the .env.example file and rename it to .env. Then, configure your environment variables accordingly.
    ```bash
    cp .env.example .env
    ```
3. **Start the Application**:

Use Docker Compose to spin up all the services:
    ```bash
    docker-compose up --build
    ```


### 🏗️ Microservices Architecture

This project is structured as microservices, with different services responsible for handling user management, NFT minting, trading, and more. Kafka is used to facilitate communication between these services.

Here are the key microservices:

	•	User Service: Handles user authentication and management.
	•	NFT Service: Manages the creation and trading of NFTs.
	•	Notification Service: Sends real-time notifications using Kafka.

### 🚀 API Documentation

API documentation is auto-generated with Swagger. You can view the available endpoints by visiting http://localhost:3000/api/docs once the server is running.

🐳 Docker & Docker Compose

The project uses Docker to containerize services for consistency across environments.

Build & Run with Docker Compose

To build and run all the services using Docker Compose, use:

docker-compose up --build
docker-compose build nft-service
docker-compose up nft-service



### 🤝 Contributing

We welcome contributions from the community! Please follow the guidelines below:

	1.	Fork the repository.
	2.	Create a new feature branch (git checkout -b feature/new-feature).
	3.	Commit your changes (git commit -m 'Add some feature').
	4.	Push to the branch (git push origin feature/new-feature).
	5.	Open a Pull Request.