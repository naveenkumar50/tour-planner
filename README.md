# 🌍 Tour Planner

A full-stack **Tour Planner application** designed to help users explore travel destinations, discover tour packages, view adventure activities, and submit travel enquiries.

The project uses a responsive frontend, a **Java backend**, and **MySQL** for data storage.

---

## ✨ Features

* 🏠 Responsive home page
* 🌍 Explore popular destinations
* 🧳 View tour packages
* 💰 Display package pricing
* 🏔️ Explore adventure activities
* 📩 Submit travel enquiries
* 🔎 Search travel options
* 💾 MySQL database integration
* ☕ Java backend
* 📱 Responsive design
* 🎨 Modern and user-friendly interface

---

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend

* Java
* JDBC

### Database

* MySQL

### Tools

* Git
* GitHub
* MySQL Workbench
* IntelliJ IDEA / Eclipse / VS Code

---

## 🏗️ Project Architecture

```text
┌─────────────────────────┐
│        Frontend         │
│                         │
│   HTML / CSS / JS       │
└────────────┬────────────┘
             │
             │ Requests
             ▼
┌─────────────────────────┐
│       Java Backend      │
│                         │
│    Business Logic       │
│    JDBC                 │
└────────────┬────────────┘
             │
             │ SQL
             ▼
┌─────────────────────────┐
│      MySQL Database     │
│                         │
│ Users / Packages /      │
│ Destinations / Enquiries│
└─────────────────────────┘
```

---

## 📂 Project Structure

```text
tour-planner/
│
├── frontend/
│   ├── index.html
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── images/
│
├── backend/
│   └── src/
│       ├── model/
│       ├── dao/
│       ├── service/
│       ├── controller/
│       └── database/
│
├── database/
│   └── tour_planner.sql
│
├── README.md
└── .gitignore
```

---

## 🗃️ Database

The project uses **MySQL** to store application data.

Create the database:

```sql
CREATE DATABASE tour_planner;
```

Example tables:

```text
users
destinations
packages
activities
bookings
contact_messages
```

---

## 🔌 Java–MySQL Connection

The Java backend connects to MySQL using **JDBC**.

Example:

```java
String url = "jdbc:mysql://localhost:3306/tour_planner";
String username = "root";
String password = "your_password";

Connection connection =
    DriverManager.getConnection(url, username, password);
```

Make sure MySQL is running before starting the Java backend.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/tour-planner.git
```

```bash
cd tour-planner
```

### 2. Create the Database

Open MySQL Workbench and create:

```sql
CREATE DATABASE tour_planner;
```

Import the SQL file:

```text
database/tour_planner.sql
```

### 3. Configure Database Credentials

Update the Java database configuration with your MySQL username, password, and database name.

### 4. Run the Java Backend

Open the backend project in your Java IDE and run the main Java application.

### 5. Run the Frontend

Open the frontend through your configured local development environment.

---

## 🔄 Application Flow

```text
User
 │
 ▼
Frontend
 │
 ▼
Java Backend
 │
 ▼
JDBC
 │
 ▼
MySQL Database
```

For example, when a user submits a contact enquiry:

```text
Contact Form
     │
     ▼
Java Backend
     │
     ▼
Validation
     │
     ▼
JDBC
     │
     ▼
MySQL
     │
     ▼
contact_messages
```

---

## 🧳 Tour Packages

The application provides travel information for destinations such as:

* 🏔️ Manali
* 🏖️ Goa
* 🕌 Jaipur
* 🌴 Kerala
* 🏛️ Delhi
* 🏞️ Darjeeling

Each package can include:

* Destination
* Package name
* Description
* Duration
* Price
* Activities
* Images

---

## 🏄 Adventure Activities

The application showcases activities such as:

* 🪂 Bungee Jumping
* 🧗 Zip Line
* 🚣 Canoeing
* 🏕️ Outdoor Adventures

---

## 🔐 Security

The Java backend should use:

* Prepared SQL statements
* Input validation
* Secure database credentials
* Password hashing
* Proper exception handling
* SQL injection prevention
* Authentication and authorization where required

---

## 🚀 Future Enhancements

* 🔐 User registration and login
* 👤 User profiles
* 🧳 Online booking
* 💳 Payment integration
* 🗺️ Maps integration
* ⭐ Reviews and ratings
* ❤️ Wishlist
* 🔎 Advanced search and filtering
* 📧 Email notifications
* 🛠️ Admin dashboard
* 📊 Booking management
* 📈 Admin analytics
* 🔗 REST API integration

---

## 🎯 Project Objectives

The main objectives of this project are:

1. Build a modern travel planning application.
2. Provide information about destinations and packages.
3. Allow users to explore adventure activities.
4. Provide a travel enquiry system.
5. Store application data using MySQL.
6. Implement backend functionality using Java.
7. Demonstrate Java–MySQL connectivity using JDBC.
8. Build a responsive and user-friendly frontend.

---

## 📚 Concepts Demonstrated

* Java
* JDBC
* MySQL
* CRUD Operations
* Object-Oriented Programming
* Database Connectivity
* HTML5
* CSS3
* JavaScript
* Responsive Web Design
* Git & GitHub

---

## ⭐ Support

If you like this project, consider giving the repository a ⭐ on GitHub.

**Plan your journey. Explore the world. 🌍✈️**
