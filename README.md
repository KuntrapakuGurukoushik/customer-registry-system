# Customer Registry System

## Project Architecture

### Project Overview

The Customer Registry System is developed to manage customer information in an organized and efficient manner. The system allows users to register customers, manage customer details, store records, and communicate using notification services.

The project follows a service-based architecture where components communicate through APIs and database services.

---

# 1. Technical Architecture

## Architecture Description

The system is divided into multiple layers to improve maintainability, scalability, and performance.

### User Interface (UI)

The User Interface allows users to interact with the application. Users can register customers, search records, update information, and access customer services.

Functions:

* Customer registration
* Data entry
* Customer profile management
* View customer records

---

### API Layer

The API acts as a communication bridge between the frontend and backend.

Functions:

* Receive requests
* Validate input
* Process responses
* Route requests to services

Example Operations:

* Register Customer
* Update Customer
* Retrieve Customer Details

---

### Services Layer

#### Registration Service

* Registers customers
* Validates customer information

#### Notification Service

* Sends notifications
* Handles SMS events

#### Customer Management Service

* Updates and retrieves customer data

---

### Database Layer

Stores customer information.

Stored Data:

* Customer ID
* Name
* Email
* Phone Number
* Address

Database Operations:

* Insert
* Update
* Delete
* Retrieve

---

### Third-Party Services

External services are integrated into the application.

Example:

* SMS Notification Service

---

## System Workflow

User
↓
User Interface
↓
API
↓
Services
↓
Database
↓
SMS Service
↓
Response

---

# 2. ER Diagram

## Entities

### Customer

Attributes:

* Customer_ID (Primary Key)
* Name
* Email
* Phone
* Address

### Notification

Attributes:

* Notification_ID (Primary Key)
* Customer_ID (Foreign Key)
* Message
* Status

Relationship:
One Customer can receive multiple notifications.

Customer (1) → (Many) Notification

---

# 3. Features

* Customer Registration
* Customer Login
* Customer Search
* Customer Profile Management
* Update Customer Details
* Notification System
* Secure Data Storage
* Customer Data Retrieval

---

# 4. Roles and Responsibilities

## Admin

* Manage customer records
* Monitor application usage

## Customer

* Register and update profile
* Access services

## API

* Process communication

## Database

* Store and manage data

## SMS Service

* Deliver notifications

---

# 5. User Flow

Open Application
↓
Register Customer
↓
Submit Customer Data
↓
API Validation
↓
Service Processing
↓
Database Storage
↓
SMS Notification
↓
Confirmation

---

# 6. MVC Pattern

## Model

Handles customer data and database operations.

## View

Displays application screens and user interactions.

## Controller

Processes user requests and manages communication between View and Model.

Flow:

View → Controller → Model → Database

---

# Technology Stack

Frontend:

* HTML
* CSS

Backend:

* Java / Python

API:

* REST API

Database:

* MySQL

Notification:

* SMS Service

---

# Advantages

* Centralized customer data
* Easy maintenance
* Scalable architecture
* Improved security
* Efficient communication

---

# Project Status

Completed:

* Project Architecture

Pending:

* Project Setup and Configuration
* Backend Development
* Database Development
* Frontend Development
* Project Execution
*
