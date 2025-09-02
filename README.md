# placement-management-system
Placement Management System – A PHP &amp; MySQL web app for managing student placements. Features include:  Admin: Manage students, companies, and placement records  Students: Update profiles, check notifications, placement status  Companies: Post opportunities, review candidates  Database: Includes SQL dump for quick setup
✨ Features
👨‍🎓 Students
Register and manage their profile
View and apply to company job postings
Check placement status and notifications

🏢 Companies
Register and log in
Post job opportunities and set eligibility criteria
View student applications and placement records

🛠️ Admin
Manage students and company accounts
Monitor placement records and statistics
Approve/reject job postings
Generate reports

📂 Project Structure
Placement-Management-System-main/
├── Admin Module/       # Admin dashboards, student & company management
├── student module/     # Student login, registration, profile mgmt
├── company module/     # Company login, job postings
├── database/           # SQL dump (placement-management.sql)
├── connection.php      # DB connection file
├── commonlogin.php     # Common login for all roles
├── registeration.php   # Registration page
└── README.md           # Project documentation

⚙️ Installation & Setup
1. Requirements
PHP 7.4+
MySQL 5.7+
Apache / XAMPP / WAMP (for local testing)
Git (to clone repo)

2. Clone Repo
git clone https://github.com/<YOUR_USERNAME>/placement-management-system.git
cd placement-management-system

3. Configure Database
Create a database:
CREATE DATABASE placement_management;

Import the dump:
mysql -u root -p placement_management < database/placement-management.sql

4. Update DB Connection
Edit connection.php (and similar config files):
<?php
$db = mysqli_connect('localhost', 'root', '', 'placement_management');
if (!$db) {
    die("Connection failed: " . mysqli_connect_error());
}
?>

5. Run Locally
Move project folder to your web root (htdocs for XAMPP).
Start Apache & MySQL.
Visit:
http://localhost/placement-management-system/commonlogin.php

🖼️ Screenshots

<img width="1007" height="714" alt="Screenshot 2025-09-02 121959" src="https://github.com/user-attachments/assets/249cfe0a-be41-4ad3-b0f4-4e9bd268596e" />





OR run built-in PHP server:

php -S localhost:8000 -t placement-management-system
