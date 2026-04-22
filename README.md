# 📊 Investment Report Builder Backend

A Spring Boot backend that helps investors generate a **single-page investment report** by simply answering a set of structured questions.

---

## 🚀 What it does

Instead of writing long notes or doing manual analysis, users:

1. Answer guided investment questions
2. Backend processes responses
3. Generates a **concise, structured report**

👉 Fast, consistent, and repeatable analysis

---

## ✨ Features

* 🔐 Google OAuth login
* 🎟️ JWT-based authentication
* 🧩 Question-driven data collection
* 📄 Single-page report generation
* 📊 Basic analytics (category insights)
* 📥 CSV-based question ingestion

---

## 🛠️ Tech Stack

* Java + Spring Boot
* Spring Security + JWT
* MySQL
* JPA / Hibernate
* Google OAuth

---

## ⚙️ Local Setup

### 1. Clone

```bash id="g3zq1x"
git clone https://github.com/your-username/investment-qna-backend.git
cd investment-qna-backend
```

---

### 2. Create local config

```bash id="m2y8kp"
src/main/resources/application-local.properties
```

```properties id="h6t2ra"
jwt.secret=your-secret
jwt.expiration=900000

spring.datasource.url=jdbc:mysql://localhost:3306/investment
spring.datasource.username=root
spring.datasource.password=your-password
```

---

### 3. Activate profile

```bash id="o1x9lf"
export SPRING_PROFILES_ACTIVE=local
```

---

### 4. Run

```bash id="z9k2pa"
./mvnw spring-boot:run
```

---

## 🔑 Environment Variables (Prod)

| Key           | Purpose     |
| ------------- | ----------- |
| JWT_SECRET    | JWT signing |
| MYSQLHOST     | DB host     |
| MYSQLPORT     | DB port     |
| MYSQLDATABASE | DB name     |
| MYSQLUSER     | DB user     |
| MYSQLPASSWORD | DB password |

---

## 📡 API Overview

### Auth

* `POST /auth/google` → Google login

### Questions

* `GET /questions` → Fetch questions

### Report

* `POST /report` → Submit answers & generate report
* `GET /report` → Retrieve report

---

## 🧠 Core Idea

> Turn scattered thinking into a structured investment report — with minimal effort.

---

## 📜 License

MIT
