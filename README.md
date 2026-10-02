# 🌍 Tour Planner

A responsive and user-friendly **Tour Planner Website** designed to help users explore popular travel destinations, discover adventure activities, view tour packages, and send travel inquiries through a contact form.

The project combines a modern frontend interface with a **PHP + MySQL backend** for handling contact form submissions.

---

## ✨ Features

* 🏠 Attractive homepage with travel-themed hero section
* 🗺️ Popular travel destinations and tour packages
* 🏔️ Adventure activities section
* 📦 Multiple travel packages with pricing
* 📱 Responsive design for desktop, tablet, and mobile
* 🔎 Search interface
* 📩 Contact/inquiry form
* 💾 MySQL database integration
* 🍔 Responsive mobile navigation menu
* 🎨 Modern UI with CSS animations and hover effects
* 🔗 Social media and contact links

---

## 🧳 Available Tour Packages

The website currently showcases packages for:

| Destination    |       Price Range |
| -------------- | ----------------: |
| 🏔️ Manali     |   ₹5,999 – ₹8,999 |
| 🏖️ Goa        |  ₹7,999 – ₹12,999 |
| 🏛️ Delhi      |   ₹2,999 – ₹8,999 |
| 🕌 Jaipur      | ₹11,999 – ₹15,999 |
| 🌴 Kerala      |   ₹4,999 – ₹9,999 |
| 🏞️ Darjeeling | ₹20,000 – ₹25,000 |

> Prices displayed on the website are sample/demo package prices.

---

## 🏄 Adventure Activities

The website provides information about popular adventure activities including:

* 🪂 Bungee Jumping
* 🧗 Zip Lines
* 🚣 Canoeing
* 🏕️ Outdoor & Adventure Experiences

---

## 🛠️ Technologies Used

### Frontend

* **HTML5**
* **CSS3**
* **JavaScript**
* **Google Fonts**
* **Font Awesome / Unicons**

### Backend

* **PHP**
* **MySQL**
* **MySQLi**

### Development Environment

* XAMPP / WAMP / LAMP
* Apache Server
* MySQL Server

---

## 📂 Project Structure

```text
tour-planner/
│
├── index.html
├── contact_us.php
│
├── css/
│   └── style.css
│
├── js/
│   └── script.js
│
├── images/
│   ├── home1.jpg
│   ├── category-1.jpg
│   ├── category-2.jpg
│   ├── category-3.jpg
│   ├── category-4.jpg
│   ├── img-1.jpg
│   ├── img-2.jpg
│   ├── img-3.jpg
│   ├── img-4.jpg
│   ├── img-5.jpg
│   ├── img-6.jpg
│   ├── serv-1.png
│   ├── serv-2.png
│   ├── serv-3.png
│   ├── serv-4.png
│   ├── serv-5.png
│   ├── serv-6.png
│   ├── footer.jpg
│   └── tick.png
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/tour-planner.git
```

Move into the project directory:

```bash
cd tour-planner
```

---

### 2. Install XAMPP

Download and install **XAMPP** if you don't already have a local PHP/MySQL environment.

Start:

* Apache
* MySQL

---

### 3. Move the Project

Copy the project folder into:

```text
C:\xampp\htdocs\
```

Your final path should look like:

```text
C:\xampp\htdocs\tour-planner\
```

---

### 4. Create the Database

Open **phpMyAdmin**:

```text
http://localhost/phpmyadmin
```

Create a database named:

```text
tour
```

Create the `contact` table using:

```sql
CREATE TABLE contact (
    id INT AUTO_INCREMENT PRIMARY KEY,
    Name VARCHAR(100) NOT NULL,
    Email VARCHAR(150) NOT NULL,
    Phone VARCHAR(20),
    Subject VARCHAR(255),
    Message TEXT
);
```

---

### 5. Configure Database Connection

The database connection is currently configured in:

```text
contact_us.php
```

Default configuration:

```php
$db_hostname = "127.0.0.1";
$db_username = "root";
$db_password = "";
$db_name = "tour";
```

If your MySQL configuration is different, update these values accordingly.

---

### 6. Run the Project

Open your browser and visit:

```text
http://localhost/tour-planner/
```

The Tour Planner website should now be running locally.

---

## 📸 Website Sections

The website contains the following main sections:

### 🏠 Home

A travel-themed landing section introducing the Tour Planner website.

### 🌄 Categories

Displays different adventure activities and experiences.

### 🧳 Packages

Shows available destinations, descriptions, and package prices.

### 📩 Contact Us

Users can submit:

* Name
* Email
* Phone
* Subject
* Message

The submitted information is stored in the MySQL database.

### 🔗 Footer

Contains:

* Quick navigation links
* Contact information
* Social media links
* Additional website links

---

## 📱 Responsive Design

The website uses CSS media queries to provide a responsive experience across:

* 💻 Desktop
* 📱 Mobile
* 📲 Tablet

The navigation menu changes to a mobile-friendly menu on smaller screens.

---

## 🔄 How the Contact Form Works

The contact form submits user information to:

```text
contact_us.php
```

PHP connects to the MySQL database and inserts the submitted information into the `contact` table.

```text
User
  │
  ▼
Contact Form
  │
  ▼
contact_us.php
  │
  ▼
PHP / MySQLi
  │
  ▼
MySQL Database
  │
  ▼
contact table
```

---

## 🚀 Future Improvements

The project can be extended with the following features:

* 🔐 User registration and login
* 👤 User profiles
* 🗓️ Online tour booking
* 💳 Online payment integration
* 🧭 Google Maps integration
* 🔍 Functional package search and filtering
* ⭐ Customer reviews and ratings
* ❤️ Wishlist/favorite destinations
* 📧 Email notifications
* 🛠️ Admin dashboard
* 📊 Booking management
* 🗃️ Dynamic packages from MySQL
* 🌐 REST API integration
* ☁️ Cloud deployment
* 🔒 Improved backend security

---

## 🔐 Security Improvements

For a production deployment, the following improvements are recommended:

* Use **prepared SQL statements**
* Validate and sanitize all form inputs
* Add CSRF protection
* Store database credentials securely
* Add server-side email validation
* Implement rate limiting for contact forms
* Disable displaying database errors to users
* Use HTTPS
* Add proper authentication and authorization

---

## 🎯 Project Goals

The main objectives of this project are to:

1. Create an attractive travel website.
2. Provide users with information about popular destinations.
3. Display travel packages and pricing.
4. Provide an easy way for users to submit travel inquiries.
5. Demonstrate frontend development using HTML, CSS, and JavaScript.
6. Demonstrate backend integration using PHP and MySQL.
7. Build a responsive website suitable for different screen sizes.

---

## 👨‍💻 Author

**Naveen Kumar**

* GitHub: [@naveenkumar50](https://github.com/naveenkumar50)
* LinkedIn: [Naveen Kumar](https://www.linkedin.com/in/naveen-kumar-498582285/)

---

## 📄 License

This project is created for **educational and demonstration purposes**.

You are free to modify and improve the project for learning and development purposes.

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub!

**Happy Travelling! 🌍✈️**
