The Online Examination System is a web application designed to manage and conduct exams online. The system allows admins to create exams, students to take exams, and both to view results. The system is developed using HTML, CSS, JavaScript, PHP, and MySQL for the database.

Features
Admin Dashboard: Manage exams, questions, and view results.
Student Dashboard: Take exams and view results.
Responsive Design: Compatible with various devices and screen sizes.
User Authentication: Secure login for both admins and students.
Real-time Feedback: Immediate results after exam submission.
Technologies Used
Frontend: HTML, CSS, JavaScript
Backend: PHP
Database: MySQL
Installation and Setup
Prerequisites
Web server (e.g., Apache)
PHP (version 7.0 or higher)
MySQL (version 5.6 or higher)
Web browser (e.g., Chrome, Firefox)
Steps to Install
Clone the Repository

bash
Copy code
git clone https://github.com/varunpratap08/online-examination-system.git

Navigate to the Project Directory

bash
Copy code
cd online-examination-system
Set Up the Database

Create a MySQL database named online_exam.
Import the database.sql file located in the sql directory to set up the necessary tables.
bash
Copy code
mysql -u root -p online_exam < sql/database.sql
Configure Database Connection

Open the config.php file located in the config directory.
Update the database connection details.
php
Copy code
<?php
$servername = "localhost";
$username = "root";
$password = "your_password";
$dbname = "online_exam";

// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>
Start the Web Server

If you are using XAMPP, place the project folder in the htdocs directory.
Start the Apache and MySQL services from the XAMPP control panel.
Access the Application

Open a web browser and navigate to http://localhost/online-examination-system.
Usage
Admin
Login
Navigate to the admin login page.
Enter the admin credentials (default: admin/admin).
Dashboard
Create new exams.
Add, update, and delete questions.
View student results.
Student
Registration and Login
Register a new account or login with existing credentials.
Dashboard
View available exams.
Take exams.
View results after submitting exams.
Directory Structure
arduino
Copy code
online-examination-system/
│
├── css/
│   ├── styles.css
│
├── js/
│   ├── scripts.js
│
├── config/
│   ├── config.php
│
├── sql/
│   ├── database.sql
│
├── admin/
│   ├── dashboard.php
│   ├── login.php
│   ├── manage_exams.php
│   ├── manage_questions.php
│
├── student/
│   ├── dashboard.php
│   ├── login.php
│   ├── register.php
│   ├── take_exam.php
│   ├── view_results.php
│
├── index.php
├── README.md
└── ...
Contributing
If you would like to contribute to the project, please follow these steps:

Fork the repository.
Create a new branch.
Make your changes and commit them.
Push to the branch.
Create a pull request.

Contact
For any queries or support, please contact [varunpratap1822@gmail.com].
