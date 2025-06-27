# 🏡 Airbnb Clone Backend

This is the backend system for an **Airbnb-like rental marketplace** application. It supports core functionalities such as user authentication, property listing, booking management, payments, reviews, and admin operations.

---

## 📌 Table of Contents
- [Features](#features)
- [System Architecture](#system-architecture)
- [Tech Stack](#tech-stack)
- [Database Models](#database-models)
- [API Overview](#api-overview)
- [Setup Instructions](#setup-instructions)
- [Testing](#testing)
- [Project Structure](#project-structure)

---

## 🚀 Features

### Core Functionalities
- **User Management** (Guests & Hosts)
- **Property Listings** with images
- **Search & Filters** by location, price, amenities
- **Booking System** with availability checks
- **Secure Payments** (Stripe, PayPal)
- **Review & Rating** system
- **Email & In-app Notifications**
- **Admin Dashboard** for moderation

### Technical Requirements
- RESTful APIs (GraphQL optional)
- JWT Authentication & RBAC
- Cloud Image Storage (e.g., AWS S3, Cloudinary)
- Email Integration (SendGrid/Mailgun)
- Global Error Handling & Logging
- Redis Caching (optional for performance)

### Non-Functional
- Scalable Architecture
- Secure Data Handling
- Performance Optimizations
- Automated Testing

---

## 🧱 System Architecture

The backend is built in a **modular and scalable architecture**, broken down into the following components:

- **API Layer**  
- **User Management**  
- **Property Listings**  
- **Booking System**  
- **Payments**  
- **Reviews**  
- **Notifications**  
- **Admin Dashboard**  
- **Authentication & RBAC**  
- **File Storage**  
- **Database Layer**  
- **Error Handling**  
- **Testing**  

For visual reference, use the provided `draw.io` diagram.

---

## 🛠️ Tech Stack

- **Language**: Python 
- **Framework**: Django 
- **Database**: PostgreSQL / MySQL
- **Authentication**: JWT, OAuth2
- **File Storage**: AWS S3 / Cloudinary
- **Payments**: Stripe / PayPal
- **Email**: SendGrid / Mailgun
- **Caching**: Redis (optional)
- **Logging**: Winston / Loguru / Sentry

---

## 🧩 Database Models

- `User`: id, name, email, role, password_hash, profile_photo  
- `Property`: id, host_id, title, description, location, price, amenities  
- `Booking`: id, guest_id, property_id, start_date, end_date, status  
- `Review`: id, booking_id, rating, comment  
- `Payment`: id, booking_id, amount, status, method

---

## 🌐 API Overview

| Method | Endpoint             | Description               |
|--------|----------------------|---------------------------|
| POST   | `/api/register`      | Register new user         |
| POST   | `/api/login`         | Authenticate user         |
| GET    | `/api/properties`    | List/search properties    |
| POST   | `/api/properties`    | Create property (host)    |
| POST   | `/api/bookings`      | Create new booking        |
| GET    | `/api/bookings/:id`  | Get booking details       |
| POST   | `/api/payments`      | Process payment           |
| POST   | `/api/reviews`       | Submit review             |

---

## 🧪 Testing

- Use `pytest` / `Jest` / [Your framework]
- Include:
  - Unit tests for models and logic
  - Integration tests for API endpoints
  - Mock tests for external services (email, payments)

---

## 🗂️ Project Structure

