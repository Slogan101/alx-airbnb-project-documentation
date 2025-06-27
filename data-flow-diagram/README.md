# 📘 Data Flow Diagram (DFD) – Airbnb Clone Backend

This document outlines the **Data Flow Diagram (DFD)** for the Airbnb Clone backend. It visualizes how data flows between external users, internal processes, and the database systems within the application.

---

## 🎯 Objective

To map the key data flows in the backend system, showing how information moves between:
- **Users (Guests, Hosts, Admins)**
- **Processes** (e.g., registration, booking, payments)
- **Data Stores** (e.g., Users, Bookings, Properties)
- **External Systems** (e.g., Payment Gateway)

This helps in planning, debugging, and scaling the backend system.

---

## 🧑‍🤝‍🧑 External Entities (Actors)

- **Guest**: A user who searches, books, and reviews properties.
- **Host**: A user who lists properties and manages bookings.
- **Admin**: Oversees users, content, and platform health.
- **Payment Gateway**: External system that handles secure transactions.

---

## 🔁 Core Processes

| ID | Process                   | Description |
|----|---------------------------|-------------|
| P1 | Register/Login User       | Handles authentication and new account creation. |
| P2 | Manage Profile            | Lets users update their profile data. |
| P3 | Manage Property Listings  | Allows hosts to create, edit, or delete listings. |
| P4 | Search & Filter Listings  | Lets guests find properties based on filters. |
| P5 | Book Property             | Handles booking requests, including date validation. |
| P6 | Process Payment           | Manages payment transactions and integration with gateway. |
| P7 | Manage Bookings           | Enables guests and hosts to cancel or view bookings. |
| P8 | Leave/Respond to Review   | Lets users add or reply to reviews after stays. |
| P9 | Admin Management          | Admin-level monitoring and moderation of data. |

---

## 🗂️ Data Stores

| ID | Data Store   | Description |
|----|--------------|-------------|
| D1 | Users        | Stores user details, roles, and credentials. |
| D2 | Properties   | Contains property listings and metadata. |
| D3 | Bookings     | Tracks all booking records and statuses. |
| D4 | Payments     | Stores payment info, status, and references. |
| D5 | Reviews      | Stores user reviews and host responses. |
| D6 | Notifications| Stores queued and sent in-app/email notifications. |

---

## 📐 DFD Layout (Suggested)

