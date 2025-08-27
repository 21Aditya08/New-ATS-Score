# ATS Score - Resume Optimizer

## 📌 Project Overview
ATS Score is a **Java-based web application** that evaluates resumes against job descriptions using AI (Gemini/OpenAI APIs). The system calculates an **ATS (Applicant Tracking System) Score** and provides personalized suggestions to improve resumes for better shortlisting chances.

The project is designed to be **interview-ready** with clean architecture, authentication, history tracking, and a modern UI/UX design.  

---

## 🚀 Features
- **Authentication & OTP Verification**
  - User registration and login
  - Email-based OTP authentication
- **Resume & Job Description Upload**
  - Upload resume files (PDF/DOCX)
  - Write or upload job description
- **ATS Score Calculation**
  - AI-powered (Gemini/OpenAI API)
  - Provides ATS match score
  - Suggests missing skills/keywords for resumes
- **History Tracking**
  - Stores user’s past job descriptions, resumes, ATS scores, and suggestions
  - View history anytime after login
- **UI/UX**
  - Minimal, smooth, mobile-first design
  - Sustainable marketplace-inspired layout
  - Warm color palette with asymmetrical layout
  - Custom eco-friendly illustrations
  - Bold expressive typography (readable & modern)
  - Micro-interactions on buttons & links
  - Fully responsive & WCAG accessible
  - Optimized for fast load times

---

## 🛠️ Tech Stack
- **Backend:** Java 17, Spring Boot, Spring Security, Hibernate, JPA
- **Frontend:** React (with TailwindCSS / Material UI)
- **Database:** PostgreSQL / MySQL
- **Authentication:** Spring Security + JWT + OTP (Email)
- **AI API Integration:** Gemini API / OpenAI API
- **Build Tool:** Maven / Gradle
- **Version Control:** GitHub (step-by-step commits for streaks)
- **Deployment:** Docker + AWS (future scope)

---

## 📂 Project Structure
```bash
ats-score/
├── backend/             # Spring Boot backend
│   ├── src/main/java/
│   ├── src/main/resources/
│   └── pom.xml
├── frontend/            # React frontend
│   ├── src/
│   ├── public/
│   └── package.json
├── docs/                # Documentation, diagrams
├── # ATS Score Spring Boot Application

A Spring Boot application for ATS (Applicant Tracking System) scoring functionality.

## Technologies Used

- **Java 17**
- **Spring Boot 3.2.0**
- **Spring Web** - For REST API endpoints
- **Spring Security** - For authentication and authorization
- **Spring Data JPA** - For data persistence
- **MySQL** - Database
- **Lombok** - To reduce boilerplate code
- **Bean Validation** - For input validation

## Project Structure

```
src/
├── main/
│   ├── java/com/example/atsscore/
│   │   ├── config/
│   │   │   └── SecurityConfig.java
│   │   ├── controller/
│   │   │   ├── AuthController.java
│   │   │   └── UserController.java
│   │   ├── dto/
│   │   │   └── UserRegistrationDto.java
│   │   ├── entity/
│   │   │   └── User.java
│   │   ├── repository/
│   │   │   └── UserRepository.java
│   │   ├── service/
│   │   │   └── UserService.java
│   │   └── AtsScoreApplication.java
│   └── resources/
│       └── application.properties
└── test/
    └── java/com/example/atsscore/
        └── AtsScoreApplicationTests.java
```

## Getting Started

### Prerequisites

- Java 17 or higher
- Maven 3.6 or higher
- MySQL 8.0 or higher

### Database Setup

1. Create a MySQL database named `ats_score_db`:
   ```sql
   CREATE DATABASE ats_score_db;
   ```

2. Update the database configuration in `src/main/resources/application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/ats_score_db
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   ```

### Running the Application

1. Clone the repository
2. Navigate to the project directory
3. Run the application:
   ```bash
   mvn spring-boot:run
   ```

The application will start on `http://localhost:8080`

### API Endpoints

#### Health Check
- **GET** `/api/auth/health` - Check if the application is running

#### User Management
- **GET** `/api/users` - Get all users (requires authentication)
- **GET** `/api/users/{id}` - Get user by ID (requires authentication)
- **POST** `/api/users` - Create a new user (requires authentication)
- **PUT** `/api/users/{id}` - Update user (requires authentication)
- **DELETE** `/api/users/{id}` - Delete user (requires authentication)

### Testing

Run the tests with:
```bash
mvn test
```

## Features

- RESTful API architecture
- Input validation using Bean Validation
- Database integration with MySQL
- Security configuration with Spring Security
- Lombok for reduced boilerplate code
- JPA entities with automatic timestamp management
- Repository pattern for data access
- Service layer for business logic

## Configuration

The application can be configured through `application.properties`:

- Database connection settings
- JPA/Hibernate configuration
- Server port configuration
- Logging levels

## Development

This is a starter template that can be extended with additional features like:
- JWT authentication
- More complex entity relationships
- File upload functionality
- Email notifications
- Advanced security configurations
- API documentation with Swagger/OpenAPI            # Project documentation
└── .gitignore
