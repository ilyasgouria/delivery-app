# Delivery App

## Overview
This repository is dedicated to the Delivery App project which aims to provide seamless delivery services using a microservices architecture.

## Architecture
The Delivery App is built using a microservices architecture. Each service is responsible for a specific function in the delivery process:
- **User Service**: Handles user authentication and profile management.
- **Order Service**: Manages the ordering process, including order placement and history.
- **Delivery Service**: Responsible for tracking and managing deliveries.
- **Notification Service**: Sends notifications to users about order status.

## Microservices
The following microservices are part of the Delivery App:
1. **User Service**
   - Handles user registration, login, and profile updates.
   - **Endpoints**:
     - `POST /api/users/register`: Register a new user.
     - `POST /api/users/login`: Log in an existing user.

2. **Order Service**
   - Manages all aspects of order processing.
   - **Endpoints**:
     - `POST /api/orders`: Place a new order.
     - `GET /api/orders/{id}`: Retrieve order details by ID.

3. **Delivery Service**
   - Handles the logistics of delivery management.
   - **Endpoints**:
     - `POST /api/deliveries`: Schedule a new delivery.
     - `GET /api/deliveries/{id}`: Track a delivery by ID.

4. **Notification Service**
   - Sends updates to users via email or SMS.
   - **Endpoints**:
     - `POST /api/notifications/send`: Send a notification to the user.

## Installation Instructions
To set up the Delivery App locally:
1. Clone the repository:
   ```bash
   git clone https://github.com/ilyasgouria/delivery-app.git
   cd delivery-app
   ```
2. Install the required dependencies:
   ```bash
   npm install
   ```
3. Start the services:
   ```bash
   npm start
   ```
4. Access the application at `http://localhost:3000`.

## Seed Data Information
The Delivery App includes seed data for initial setup. To load the seed data:
1. Run the following command:
   ```bash
   npm run seed
   ```
2. This will populate the database with initial users, orders, and delivery information.

For any additional information or troubleshooting, please consult the [Wiki](https://github.com/ilyasgouria/delivery-app/wiki).