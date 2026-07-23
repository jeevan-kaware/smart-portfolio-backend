# 🚀 Smart Portfolio Backend

<div align="center">

# 💼 Smart Portfolio Backend

### AI-Powered Portfolio Backend built with Spring Boot, Spring AI and Google Gemini

<p align="center">

<img src="https://img.shields.io/badge/Java-21-red?style=for-the-badge&logo=openjdk&logoColor=white"/>

<img src="https://img.shields.io/badge/Spring_Boot-3.5-green?style=for-the-badge&logo=springboot"/>

<img src="https://img.shields.io/badge/Spring_AI-Google_Gemini-blue?style=for-the-badge"/>

<img src="https://img.shields.io/badge/Google-Gemini_2.5_Flash-4285F4?style=for-the-badge&logo=google&logoColor=white"/>

<img src="https://img.shields.io/badge/PostgreSQL-Database-blue?style=for-the-badge&logo=postgresql"/>

<img src="https://img.shields.io/badge/REST-API-success?style=for-the-badge"/>

<img src="https://img.shields.io/badge/Maven-Build-red?style=for-the-badge&logo=apachemaven"/>

<img src="https://img.shields.io/badge/Docker-Supported-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>

<img src="https://img.shields.io/badge/Render-Deployed-46E3B7?style=for-the-badge&logo=render&logoColor=white"/>

<img src="https://img.shields.io/badge/JSON-API-black?style=for-the-badge"/>

</p>

</div>

---

# 📖 Overview

Smart Portfolio Backend is a production-ready REST API built using **Spring Boot**, **Spring AI**, and **Google Gemini** that powers my personal developer portfolio.

The backend exposes REST APIs for portfolio information, AI-powered chat, contact form handling, and health monitoring. It follows a clean layered architecture and is designed to serve a modern frontend application.

The project integrates **Spring AI** with **Google Gemini 2.5 Flash** to provide an intelligent portfolio assistant capable of answering questions about my skills, projects, education, certifications, and experience.

The backend also includes a Contact API with email service integration, allowing visitors to submit messages directly from the portfolio website.

The application is containerized using **Docker**, configured with environment variables, deployed on **Render**, and designed to integrate seamlessly with the React frontend hosted on **Vercel**.

---

# 🌐 Live Demo

## 💼 Portfolio

https://smart-portfolio-kappa-eight.vercel.app/

---

## ⚙ Backend API

https://ai-model-comparison-sym8.onrender.com

---

## 📂 Repository

https://github.com/jeevan-kaware/smart-portfolio-backend

---

# ✨ Features

## 🤖 AI Portfolio Assistant

- Google Gemini 2.5 Flash Integration
- Spring AI Integration
- AI-powered Portfolio Chat
- Context-aware Responses
- Portfolio Information Assistant
- Skills & Project Queries
- Short and Accurate Responses
- Prompt-based AI Interaction

---

## 📬 Contact Form API

- Contact Form Submission
- Email Notification Support
- Reply-To Email Support
- Request Validation
- Backend Email Service Integration
- JSON Request Processing
- REST API Response

---

## 💼 Portfolio Backend

- Portfolio Information API
- Health Check API
- RESTful Endpoints
- JSON Responses
- Cross-Origin Configuration
- Environment Variable Support
- Frontend Integration

---

## 🔒 Backend Features

- Layered Architecture
- DTO Pattern
- Service Layer
- Configuration Layer
- Validation
- Exception-safe API Design
- Dependency Injection
- Clean Code Structure

---

## 🐳 Deployment Features

- Docker Support
- Multi-stage Docker Build
- Environment Variables
- Render Deployment
- Production-ready Configuration

---

# 🛠 Tech Stack

| Technology | Used |
|------------|------|
| Java 21 | ✅ |
| Spring Boot 3.5 | ✅ |
| Spring AI | ✅ |
| Google Gemini 2.5 Flash | ✅ |
| Spring Web | ✅ |
| Spring Validation | ✅ |
| Java Mail | ✅ |
| Maven | ✅ |
| Docker | ✅ |
| REST API | ✅ |
| Render | ✅ |

---

# 🧩 Project Architecture

```text
                Portfolio Website

                        │

                        ▼

              Spring Boot REST API

                        │

        ┌───────────────┼────────────────┐

        ▼               ▼                ▼

 AI Chat API      Contact API      Health API

        │               │

        ▼               ▼

 Spring AI       Email Service

        │

        ▼

 Google Gemini 2.5 Flash
```

---

# 🚀 Backend Workflow

```text
Frontend Request

        │

        ▼

REST Controller

        │

        ▼

Service Layer

        │

        ▼

Spring AI / Email Service

        │

        ▼

Response Returned

        │

        ▼

Portfolio Frontend
```

---

# 📡 REST API Endpoints

## 🤖 AI Chat API

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/chat` | AI Portfolio Assistant |

---

## 📬 Contact API

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/contact` | Submit Portfolio Contact Form |

---

## ❤️ Health API

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/api/health` | Backend Health Status |

---

# 🛡 Backend Highlights

The backend follows modern Spring Boot development practices.

Features included

- Spring AI Integration
- Google Gemini Integration
- Layered Architecture
- DTO Pattern
- Email Service
- Request Validation
- REST API Design
- Docker Support
- Environment Variables
- Render Deployment
- Production-ready Project Structure

--- 
# 📂 Project Structure

```text
src
│
├── config
│   ├── MailConfig
│   └── WebConfig
│
├── controller
│   ├── ChatController
│   ├── ContactController
│   └── HealthController
│
├── dto
│   ├── ChatRequest
│   ├── ChatResponse
│   └── ContactRequest
│
├── service
│   ├── ChatService
│   ├── EmailService
│   └── impl
│       └── EmailServiceImpl
│
└── PortfolioBackendApplication
```

---

# 🔄 Request Flow

```text
Portfolio Frontend

        │

        ▼

REST Controller

        │

        ▼

Validation

        │

        ▼

Service Layer

        │

   ┌────┴─────┐

   ▼          ▼

Spring AI   Email Service

   ▼          ▼

Google Gemini   SMTP Mail

        │

        ▼

JSON Response
```

---

# ⚙️ Getting Started

## 1️⃣ Clone Repository

```bash
git clone https://github.com/jeevan-kaware/smart-portfolio-backend.git
```

```bash
cd smart-portfolio-backend
```

---

## 2️⃣ Configure Environment Variables

Create an **application.properties** file or configure environment variables.

```properties
spring.application.name=portfolio-backend

server.port=${PORT:8080}

spring.ai.google.genai.api-key=YOUR_GEMINI_API_KEY

spring.ai.google.genai.chat.options.model=gemini-2.5-flash

MAIL_USERNAME=YOUR_EMAIL

MAIL_PASSWORD=YOUR_APP_PASSWORD

app.cors.origins=http://localhost:5173,https://smart-portfolio-kappa-eight.vercel.app
```

---

## 3️⃣ Run the Project

Using Maven

```bash
./mvnw spring-boot:run
```

or

```bash
mvn spring-boot:run
```

---

Backend starts on

```text
http://localhost:8080
```

---

# 🐳 Docker Support

The project includes a production-ready multi-stage Dockerfile.

Build Docker Image

```bash
docker build -t smart-portfolio-backend .
```

Run Container

```bash
docker run -p 8080:8080 smart-portfolio-backend
```

---

# ☁ Deployment

The backend is deployed on **Render**.

Live Backend API

```text
https://ai-model-comparison-sym8.onrender.com
```

Portfolio Frontend

```text
https://smart-portfolio-kappa-eight.vercel.app/
```

---

# 🌍 API Examples

## 🤖 AI Portfolio Assistant

Request

```http
POST /api/chat
```

```json
{
  "message": "What are Jeevan's top skills?"
}
```

Response

```json
{
  "reply": "Jeevan's skills include Java, Spring Boot, Spring Security, Spring AI, PostgreSQL, Docker, Git, GitHub, HTML, CSS, JavaScript and React (Basics)."
}
```

---

## 📬 Contact Form

Request

```http
POST /api/contact
```

```json
{
  "name":"John Doe",
  "email":"john@example.com",
  "message":"I would like to connect with you."
}
```

Response

```json
{
   "success": true,
   "message": "Message sent successfully."
}
```

---

## ❤️ Health Check

Request

```http
GET /api/health
```

Response

```json
{
   "status":"UP",
   "service":"portfolio-backend"
}
```

---

# 🤖 AI Assistant Workflow

```text
Visitor asks a question

          │

          ▼

Portfolio Frontend

          │

          ▼

POST /api/chat

          │

          ▼

Spring Boot Backend

          │

          ▼

Spring AI

          │

          ▼

Google Gemini 2.5 Flash

          │

          ▼

AI Response Generated

          │

          ▼

Displayed on Portfolio
```

---

# 📬 Contact Workflow

```text
Visitor fills Contact Form

            │

            ▼

Frontend

            │

            ▼

POST /api/contact

            │

            ▼

Validation

            │

            ▼

Email Service

            │

            ▼

Email Sent Successfully
```

---

# 🌟 Highlights

- Google Gemini AI Integration
- AI Portfolio Assistant
- Contact Form API
- Email Service Integration
- Health Monitoring API
- Layered Architecture
- DTO Pattern
- Docker Support
- Render Deployment
- Production-ready REST APIs
- Clean Project Structure
- Environment Variable Configuration

---
# 📚 Learning Outcomes

This project helped me gain practical experience with:

- Java 21
- Spring Boot 3
- Spring AI
- Google Gemini API Integration
- Prompt Engineering
- REST API Development
- Layered Architecture
- DTO Pattern
- Dependency Injection
- Bean Validation
- Java Mail Integration
- CORS Configuration
- Environment Variables
- Docker
- Multi-stage Docker Build
- Render Deployment
- Maven
- JSON API Development
- Backend & Frontend Integration
- Production Deployment
- Clean Code Practices

---

# 🚀 Future Improvements

The project can be extended with additional enterprise-level features:

- JWT Authentication
- Spring Security
- User Login & Registration
- Portfolio Admin Dashboard
- Database Integration
- Chat History
- Conversation Memory
- Streaming AI Responses
- Markdown Rendering
- Resume Analyzer
- AI Resume Review
- AI Project Recommendation
- Multi-language Support
- OpenAI Integration
- Claude Integration
- Groq Integration
- Ollama Integration
- DeepSeek Integration
- OpenRouter Support
- Redis Cache
- Docker Compose
- Kubernetes Deployment
- CI/CD Pipeline
- Monitoring & Logging
- Unit & Integration Testing

---

# 🤝 Contributing

Contributions are welcome!

If you'd like to improve this project:

1. Fork the repository
2. Create a new feature branch
3. Commit your changes
4. Push your branch
5. Open a Pull Request

---

# 👨‍💻 Author

## Jeevan Kaware

**Java Backend Developer | Spring Boot Developer**

### 🔗 GitHub

https://github.com/jeevan-kaware

---

### 📂 Backend Repository

https://github.com/jeevan-kaware/smart-portfolio-backend

---

### 🌐 Live Backend

https://ai-model-comparison-sym8.onrender.com

---

### 💼 Portfolio

https://smart-portfolio-kappa-eight.vercel.app/

---

### 💼 LinkedIn

https://www.linkedin.com/in/jeevan-kaware-080643355

---

# ⭐ Support

If you found this project helpful, please consider giving it a ⭐ on GitHub.

Your support motivates me to continue building production-ready Java Backend, Spring Boot, and AI-powered applications.

---

<div align="center">

# 🚀 Built with Java, Spring Boot, Spring AI, Google Gemini, Docker and ❤️

### Thank you for visiting this repository!
