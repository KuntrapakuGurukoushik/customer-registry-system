# Customer Registry System

## Project Overview

The Customer Registry System is designed to store and manage customer information efficiently. The system uses a service-based architecture where different components communicate through APIs and database services.

## Technical Architecture

The system consists of the following components:

* **User Interface (UI):** Allows users to interact with the application.
* **API:** Receives HTTP requests and transfers data to services.
* **Services:** Handles business logic including customer registration and notifications.
* **Database:** Stores customer information.
* **Third-Party Service:** SMS service for sending notifications.

### System Flow

User → User Interface → API → Services → Database → SMS Service → Response

## ER Diagram

Entities used in the system:

### Customer

* Customer_ID
* Name
* Email
* Phone
* Address

### Notification

* Notification_ID
* Customer_ID
* Message
* Status

Relationship:
One Customer can receive multiple notifications.

## Project Status

Completed:

* Technical Architecture
* ER Diagram

Pending:

* Features
* Roles and Responsibilities
* User Flow
* MVC Pattern
* Backend Development
* Frontend Development
*
