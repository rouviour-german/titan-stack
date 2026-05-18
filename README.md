# TitanStack: FastAPI & React Multi-Tenancy Enterprise Template

A modern, high-performance full-stack Multi-tenant application template. Featuring a FastAPI backend with Clean Architecture, a React frontend with TypeScript, and a comprehensive suite of tools for rapid development and scalable deployment.

## ✨ Key Features

### 🔐 User Management
- **Enterprise Auth**: JWT-based authentication with secure refresh token cycles.
- **Biometric Login**: Native Passkeys (WebAuthn) support for passwordless security.
- **Magic Links**: Seamless login via secure email links.
- **SSO Integration**: Configurable Single Sign-On capabilities.
- **Granular Profiles**: Complete user management with image uploads and account status control.

### 🏢 Multi-Tenancy
- **Data Isolation**: Robust multi-tenancy support ensuring data security per tenant.
- **Advanced Routing**: Support for subdomains and custom white-label domains.
- **Tenant Administration**: Full CRUD for tenant life-cycle management.
- **Search & Discovery**: Tenant search functionality by subdomain and name.

### 🏢 Role-Based Access Control (RBAC)
- **Dynamic Permission Matrix**: Fine-grained control over system features.
- **Custom Roles**: Create and assign tenant-specific roles.
- **Hierarchical Permissions**: Inherited and overridden permission levels.

### 💳 Stripe & Billing
- **Subscription Engine**: Manage monthly/yearly billing cycles.
- **Product Management**: Full-featured product and pricing plan CRUD.
- **Invoicing**: Automated invoice generation and tracking.
- **Trial Systems**: Configurable trial periods for all subscription plans.

### 🤖 AI Integration
- **Local LLM Support**: Integration with local AI models (Ollama).
- **Streaming Responses**: Real-time AI chat interface with low latency.
- **Conversation Context**: Persistent chat history and model selection.

### ☁️ Infrastructure & Storage
- **Cloud Storage**: Native support for Azure Blob and AWS S3 compatible storage.
- **File Processing**: Secure upload validation and multi-provider abstraction.
- **Dockerized**: Fully containerized environment for dev and prod.

---

## 🏗️ Architecture Overview

TitanStack follows **Clean Architecture** principles, separating business logic from infrastructure to ensure long-term maintainability.

### Tech Stack

- **Backend**: FastAPI, MongoDB (Beanie ODM), Redis, Celery (Async Tasks).
- **Frontend**: React 18, TypeScript, Vite, Tailwind CSS, shadcn/ui.
- **Infrastructure**: Docker, Docker Compose, Kubernetes (Helm).

---

## 🔧 Getting Started

### Prerequisites
- Python 3.13+
- Node.js 22+
- Docker & Docker Compose
- pnpm

### Initial Setup

1. **Backend Environment**:
   ```bash
   cp backend/.env.example backend/.env
   # Edit backend/.env with your credentials
   ```

2. **Infrastructure Services**:
   ```bash
   docker-compose -f dev.compose.yaml up -d
   ```

3. **Backend Development**:
   ```bash
   cd backend
   uv sync
   uv run fastapi dev api
   ```

4. **Frontend Development**:
   ```bash
   cd frontend/app
   pnpm install
   pnpm dev
   ```

### Accessing Services
- **Backend API**: `http://localhost:8000`
- **Frontend App**: `http://localhost:5173`
- **API Documentation**: `http://localhost:8000/docs`
- **Fake SMTP UI**: `http://localhost:1083`

---

---

## Author & Contact

- **GitHub:** [@rouviour-german](https://github.com/rouviour-german)
- **Email:** [rouviourgermanmeetings@gmail.com](mailto:rouviourgermanmeetings@gmail.com)
- **Profile:** https://github.com/rouviour-german

