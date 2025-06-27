# 📘 Use Case Diagram - Airbnb Clone Backend

This document provides an overview of the **Use Case Diagram** for the Airbnb Clone backend system. It visualizes the key **interactions between users and the system**, including user registration, property listings, bookings, payments, and admin operations.

---

## 🎯 Objective

To map out how different types of users (actors) interact with the system using a **use case diagram**, supporting the design and development of backend features.

---

## 🧑‍🤝‍🧑 Actors

- **Guest**: A user looking to browse and book properties.
- **Host**: A user listing and managing rental properties.
- **Admin**: System administrator managing platform data and users.
- **Payment Gateway** (external): Processes payments and handles payouts.

---

## 🎮 Use Cases

### Guest
- Register an account
- Log in / Authenticate
- Search and filter properties
- View property details
- Book a property
- Cancel a booking
- Make a payment
- Leave a review
- Receive notifications

### Host
- Register as host
- Log in / Authenticate
- Create/edit/delete property listings
- View guest bookings
- Cancel bookings
- Respond to guest reviews
- Receive payments

### Admin
- Manage users (approve, ban, verify)
- Manage listings (approve/delete)
- Monitor bookings
- Oversee payment activity
- Generate system reports
- Send platform-wide notifications

### Payment Gateway (External System)
- Process payments
- Trigger host payouts
- Notify backend of payment status

---


