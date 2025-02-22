# Contact Form with Email & Database (PHP + MySQL)

## 📌 Introduction
This project is a simple **contact form** that allows users to send messages via email and store them in a MySQL database.

## 🛠 Technologies Used
- PHP
- MySQL
- PHPMailer (for email functionality)

## 🚀 Setup & Installation
### 1️⃣ Prerequisites
- A web server (Apache, Nginx, etc.)
- PHP 7 or later
- MySQL database
- PHPMailer library (install via Composer)

### 2️⃣ Clone the Repository
```sh
git clone https://github.com/yourusername/ContactFormPHP.git
cd ContactFormPHP
```

### 3️⃣ Install Dependencies
```sh
composer require phpmailer/phpmailer
```

### 4️⃣ Database Setup
1. Create a MySQL database:
```sql
CREATE DATABASE contact_form;
USE contact_form;
CREATE TABLE messages (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    message TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```
2. Update database credentials in `contact_form.php`:
```php
$servername = "your_server";
$username = "your_username";
$password = "your_password";
$dbname = "contact_form";
```

### 5️⃣ Run the Application
1. Start your web server.
2. Open `contact_form.php` in a browser.
3. Fill out the form and submit it.

## 📢 Contributing
Feel free to fork and contribute! Open an issue if you find any bugs. 😊

## 📜 License
This project is licensed under the MIT License.

