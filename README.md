# Smart Email Generator ✉️🤖

A robust, enterprise-grade backend application built using **Java 21** and **Spring Boot** that automates and generates contextual email structures using RESTful APIs.

## 🚀 Tech Stack & Core Dependencies
* **Language:** Java 21
* **Framework:** Spring Boot 3.x
* **Core Modules:** Spring Web (REST APIs), Spring Boot DevTools
* **Build Tool:** Maven

## 🛠️ Architecture & Features
* **REST Endpoints:** Structured controllers mapping requests natively to process contextual input data.
* **Service Layer Separation:** Implements a decoupled service layer to handle the processing logic separate from the web layer.
* **Error Handling:** Centralized exception handling to ensure consistent JSON responses for API failures.

## 📋 API Endpoints
### Generate a New Email
* **URL:** `/api/v1/email/generate`
* **Method:** `POST`
* **Request Body:**
```json
{
  "sender": "yourname@example.com",
  "recipient": "hr@company.com",
  "subject": "Application for Java Backend Role",
  "prompt": "Write a professional follow-up email regarding my application status."
}
```
* **Success Response (200 OK):**
```json
{
  "status": "success",
  "generatedEmail": "Dear HR Team,\n\nI hope this email finds you well..."
}
```

## 💻 How to Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Navigate to the project directory:
   ```bash
   cd smart-email-generator
   ```
3. Run the application using Maven:
   ```bash
   ./mvnw spring-boot:run
   ```
4. Access the API locally at: `http://localhost:8080`
