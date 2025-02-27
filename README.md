# Online Flight Booking System

## Description
The Online Flight Booking System is a web-based application built using PHP and MySQL, designed to allow users to book flights, view available flights, and manage their bookings.

## Features
- User Registration & Login
- Flight Search & Booking
- Admin Panel for Managing Flights
- Payment Integration (if applicable)
- Email Notifications (using PHPMailer)

## Technologies Used
- PHP
- MySQL
- XAMPP (Apache, MySQL, PHP)
- HTML, CSS, JavaScript
- Bootstrap (optional for UI enhancements)

## Installation & Setup

### 1. Install XAMPP
Download and install XAMPP from [Apache Friends](https://www.apachefriends.org/index.html).

### 2. Start Apache & MySQL
- Open XAMPP Control Panel
- Start **Apache** and **MySQL** services

### 3. Set Up Database
- Open **phpMyAdmin** (`http://localhost/phpmyadmin/`)
- Create a new database: `DATABASE FILE`
- Import the provided SQL file (`ofbsphp.sql`) into the database

### 4. Configure Database Connection
- Locate the `config.php` file in your project directory
- Update the database credentials:
  ```php
  $servername = "localhost";
  $username = "root";
  $password = "";
  $dbname = "DATABASE FILE";
  ```

### 5. Set Up the Project in XAMPP
- Copy the project folder to `C:\xampp\htdocs\Online-Flight-Booking`
- Open a browser and visit `http://localhost/Online-Flight-Booking/`

### 6. Configure PHPMailer (For Email Notifications)
- Open `mail_config.php`
- Update SMTP settings (e.g., Gmail SMTP):
  ```php
  $mail->Host = 'smtp.gmail.com';
  $mail->SMTPAuth = true;
  $mail->Username = 'your-email@gmail.com';
  $mail->Password = 'your-email-password';
  $mail->SMTPSecure = PHPMailer::ENCRYPTION_STARTTLS;
  $mail->Port = 587;
  ```

### 7. Run the Application
- Open a browser and visit `http://localhost/Online-Flight-Booking/`
- Register an account and start booking flights

## GitHub Repository
Find the source code here: [Online Flight Booking GitHub](https://github.com/Swathi251105/Online-Flight-Booking)


## Troubleshooting
- If you face database connection errors, check your `config.php` settings.
- If Apache or MySQL doesn’t start, check if other applications (like Skype) are using port 80 or 3306.
- Enable debugging in PHP by modifying `php.ini` (`display_errors = On`).

## License
This project is open-source under the MIT License.

