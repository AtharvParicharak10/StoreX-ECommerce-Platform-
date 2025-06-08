
# Java Microservices eCommerce Platform Documentation

Welcome to the documentation for the **Microservices-based eCommerce Platform** built using Spring Boot. This platform is designed to be modular, scalable, and efficient, with a clear separation of concerns between services.

---

## 🚀 Overview

This platform includes the following key microservices:

- **Product Catalog Service**
- **Payment Gateway Integration Service**
- **Order Management Service**
- **Notification (Email) Service**

Each service is independently deployable, communicates via REST and event-driven messaging, and is backed by robust persistence and caching mechanisms.

---

## 🔧 Technologies Used

- **Spring Boot** – Core framework
- **Spring Data JPA & Hibernate** – Database persistence
- **Redis** – Caching layer
- **MySQL/PostgreSQL** – Relational databases
- **JWT & OAuth2** – Security and authentication
- **RabbitMQ/Kafka** – Event-driven architecture support
- **Docsify** – Live documentation

---

## 🧩 Microservices Breakdown

### 📦 Product Catalog Service

Manages product data including creation, updates, deletion, and search.

**Features:**

- CRUD operations
- Pagination and sorting
- Search by category or name

**Tech:** Spring Boot, JPA, MySQL

---

### 💰 Payment Gateway Integration Service

Handles secure transactions via external payment processors.

**Features:**

- Payment initiation and status tracking
- Retry and fallback mechanisms

**Tech:** REST APIs, Secure token handling

---

### 🧾 Order Management Service

Responsible for order placement, tracking, and status updates.

**Features:**

- Cart management
- Order creation
- Integration with Product and Payment services

**Tech:** Spring Boot, JPA, Kafka

---

### ✉️ Notification (Email) Service

An event-driven service for sending emails at scale.

**Features:**

- Templated transactional emails
- Event-based triggers via messaging queue
- Scalable and asynchronous processing

**Tech:** Spring Boot, RabbitMQ, HTML Email Templates

---

## 📈 Performance Optimization

- **API Response Optimization:** Reduced response time from **500 ms to 50 ms** using Redis caching.
- **Efficient Pagination:** Implemented dynamic pagination & sorting for large datasets.
- **Database Efficiency:** Hibernate & JPA optimizations to prevent N+1 query issues.

---

## 🔐 Security Highlights

- **JWT Authentication** – Stateless user sessions
- **OAuth2 Integration** – Secure access delegation
- **Role-based Authorization** – Fine-grained control over endpoints

---

## 📡 API Design

- RESTful principles followed strictly
- Standard HTTP methods: `GET`, `POST`, `PUT`, `DELETE`
- JSON-based payloads

---

## 📚 Documentation Setup with Docsify

This project uses **Docsify** to serve documentation in real-time.

### How to Run:

```bash
npm install -g docsify-cli

# From project root
docsify init docs
cd docs

# Start local server
docsify serve .
```

Then open: [http://localhost:3000](http://localhost:3000)

---

## 📁 Folder Structure (docs)

```
docs/
├── index.html
├── README.md
├── _sidebar.md
└── services/
    ├── product-service.md
    ├── payment-service.md
    ├── order-service.md
    └── email-service.md
```

---

## 📝 Credits

Developed and documented by: **Atharv P.**
