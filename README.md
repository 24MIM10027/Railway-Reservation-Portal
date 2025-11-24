# Railway-Reservation-Portal

📌 Project Title

Railway Reservation Portal

📘 Overview

The Railway Reservation Portal is a Java-based system designed to provide a complete solution for train search, seat availability checking, reservation, ticket management, and administrative operations.
The project demonstrates modular software development, layered architecture, database-driven workflows, error handling, and proper documentation practices.

Users can search for trains, check available seats, book tickets, view booking history, and manage reservations.
Administrators can manage trains, schedules, and routes, and view booking reports.
The system follows a clean MVC-style structure and applies essential software engineering concepts such as UML diagrams, ER modeling, concurrency control, and validation.

✨ Features
User Features

-Account registration & login

-Train search by source, destination, and travel date

-Real-time seat availability

-Ticket booking with confirmation

-Automatic waitlist assignment when seats are full

-View booking history

-Cancel bookings

-Admin Features

-Create/update trains and schedules

-Manage routes and seat capacity

-View booking reports and analytics

-System Features

-Layered architecture (Controller → Service → Repository → DB)

-Transactional seat allocation to prevent overbooking

-Centralized exception handling

-Logging for critical operations

-Modular design with 5–10 meaningful Java classes

-Unit testing support

🛠️ Technologies / Tools Used

Java (Core + OOP concepts)

Spring Boot

MySQL

Spring Data JPA (Hibernate)

Maven

JUnit 5 & Mockito (testing)

Draw.io / UML tools

Git & GitHub

📂 Project Structure
RailwayReservationPortal/
│── src/
│   ├── main/java/com/railwayportal/
│   │   ├── controller/
│   │   ├── service/
│   │   ├── repository/
│   │   ├── entity/
│   │   ├── dto/
│   │   ├── util/
│   │   ├── exception/
│   │   └── RailwayReservationPortalApplication.java
│   │
│   ├── main/resources/
│   │   ├── application.properties
│   │   ├── static/
│   │   └── templates/
│── tests/
│── docs/
│── README.md
│── statement.md

🚀 How to Install & Run the Project
1. Clone the Repository
git clone <your-repository-url>
cd RailwayReservationPortal

2. Configure the Database

Create a MySQL database:

CREATE DATABASE railway_portal;


Update application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/railway_portal
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

3. Build & Run the Application
mvn clean install
mvn spring-boot:run

4. Access the Application

REST API: http://localhost:8080/api/...

Web UI (if used): http://localhost:8080/

🧪 Testing Instructions

Run all test cases using:

mvn test


Includes:

Booking logic tests

Seat availability tests

Admin module tests

Database interaction tests

📌 Major Modules Implemented

Authentication Module

Search & Availability Module

Booking Module

Route & Schedule Management Module

Admin Reporting Module

💡 Future Enhancements

Integration with an online payment gateway

Real-time seat map visualization

Dynamic pricing system

Mobile app interface

Notification system for booking status

👤 Author

Name: N Raja Ravi Varma
Register Number: 24MIM10027
Course: Programming in Java
