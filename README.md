# 🚆 Railway Reservation Portal — Using Java Programming

The **Railway Reservation Portal** is a Java-based system designed to provide a complete solution for train search, seat availability checking, reservation, ticket management, and administrative operations.  
The project follows modular software development practices, layered architecture, database-driven workflows, clean MVC structure, concurrency-safe booking logic, and includes proper documentation with UML diagrams and ER modeling.

Users can search for trains, check available seats, book tickets, view booking history, and manage reservations.  
Administrators can manage trains, routes, schedules, and view booking reports.

---

## ✨ Features

### **User Features**
- Account registration & login  
- Train search by source, destination, and travel date  
- Real-time seat availability display  
- Ticket booking with seat confirmation  
- Automatic waitlist assignment when seats are full  
- View booking history  
- Cancel booked tickets  

### **Admin Features**
- Create, update, and delete trains  
- Manage route & station configurations  
- Define and update train schedules  
- Modify seat capacity  
- View booking reports and occupancy analytics  

### **System Features**
- Layered architecture (Controller → Service → Repository → Database)  
- Transaction-safe seat allocation (prevents overbooking)  
- Centralized exception handling  
- Logging for all important operations  
- Modular design with reusable OOP components  
- Unit testing support using JUnit 5 & Mockito  
- Cleanly documented with UML diagrams, ER diagrams, and workflow charts  

---

## 🛠️ Technologies / Tools Used

- **Java 17+**  
- **Spring Boot 3.x**  
- **Spring Web**  
- **Spring Data JPA (Hibernate)**  
- **MySQL 8.x**  
- **Maven**  
- **JUnit 5 & Mockito** (testing)  
- **Draw.io** (UML & ER diagrams)  
- **Git & GitHub**  
- **Postman** (API testing)

---

## 📂 Project Structure
```
RailwayReservationPortal/
│── src/
│ ├── main/java/com/railwayportal/
│ │ ├── controller/ # REST controllers
│ │ ├── service/ # Business logic
│ │ ├── repository/ # JPA repositories
│ │ ├── entity/ # JPA entity classes
│ │ ├── dto/ # Request/response DTOs
│ │ ├── util/ # Utility helpers
│ │ ├── exception/ # Global exception handling
│ │ └── RailwayReservationPortalApplication.java
│ │
│ ├── main/resources/
│ │ ├── application.properties # Database configuration
│ │ ├── static/ # Frontend assets (optional)
│ │ └── templates/ # Thymeleaf templates (optional)
│ │
│ └── test/java/com/railwayportal/
│ └── service/ # Unit tests
│
│── sql/ # SQL schema & seed data
│── docs/ # UML diagrams, ER diagrams, report
│── README.md
│── statement.md
```

---

## 🚀 How to Install & Run the Project

### **1. Clone the Repository**
```bash
git clone <your-repository-url>
cd RailwayReservationPortal
```
### **2. Configure MySQL**

Create the database:
```sql

CREATE DATABASE railway_portal;
```

### Update application.properties:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/railway_portal
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### **3. Build & Run the Application**
```bash
mvn clean install
mvn spring-boot:run
```

### **4. Access the Application**

-**REST API:** http://localhost:8080/api/ (still on working condition)

-**Web UI (if using Thymeleaf):** http://localhost:8080/ (still on working condition)

## 🧪 Testing Instructions

Run all test cases:
```bash
mvn test
```

### Includes:

-Booking logic tests

-Seat availability tests

-Waitlist promotion tests

-Train search tests

-Admin module tests

## 📌 Major Modules Implemented

-Authentication Module

-Search & Availability Module

-Booking Module (seat allocation + waitlist)

-Route & Schedule Management Module

-Admin Reporting Module

## 💡 Future Enhancements

-Integration with online payment gateway

-Real-time seat map visualization

-Mobile application version

-Dynamic ticket pricing

-Notification system (SMS/Email)

## 👤 Author

**Name:** N Raja Ravi Varma
