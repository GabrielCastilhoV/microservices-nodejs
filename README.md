# Microservices Node.js Project

A microservices architecture built with Node.js, TypeScript, and modern web technologies.

## 🏗️ Architecture

This project consists of multiple microservices:

- **app-orders**: Order management service
- **app-invoices**: Invoice management service
- **infra**: Infrastructure as Code using Pulumi
- **contracts**: Shared message contracts between services

## 🚀 Tech Stack

- **Language**: TypeScript
- **Framework**: Fastify
- **Database**: PostgreSQL with Drizzle ORM
- **Message Broker**: RabbitMQ
- **API Gateway**: Kong
- **Infrastructure**: Pulumi
- **Observability**: OpenTelemetry
- **Validation**: Zod

## 📁 Project Structure

```
├── app-orders/          # Order management microservice
├── app-invoices/        # Invoice management microservice
├── contracts/           # Shared message contracts
├── infra/               # Infrastructure as Code
└── docker/              # Docker configurations
```

## 🛠️ Getting Started

### Prerequisites

- Node.js 22+
- Docker & Docker Compose
- PostgreSQL
- RabbitMQ

### Installation

1. Clone the repository
2. Install dependencies for each service:

   ```bash
   cd app-orders && npm install
   cd ../app-invoices && npm install
   cd ../infra && npm install
   ```

3. Start the infrastructure:

   ```bash
   docker-compose up -d
   ```

4. Run services in development mode:

   ```bash
   # Terminal 1
   cd app-orders && npm run dev

   # Terminal 2
   cd app-invoices && npm run dev
   ```

## 🔧 Development

### Available Scripts

- `npm run dev`: Start service in development mode with hot reload
- `npm run start`: Start service in production mode

## 🐳 Docker

Use the provided Docker Compose files to run the complete stack locally.

## 📊 Monitoring

OpenTelemetry integration provides distributed tracing and metrics collection.
