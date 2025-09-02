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
<img width="1063" height="631" alt="Screenshot 2025-09-02 122121" src="https://github.com/user-attachments/assets/7b53e8b4-231a-4f8b-87c1-c8f70e9ae3c8" />
<img width="927" height="555" alt="Screenshot 2025-09-02 122105" src="https://github.com/user-attachments/assets/3bf198fa-4746-4343-a326-f6c57c51678b" />
<img width="790" height="833" alt="Screenshot 2025-09-02 122054" src="https://github.com/user-attachments/assets/07829a82-e4c2-4b7b-a5af-26c3db7015ee" />
<img width="551" height="693" alt="Screenshot 2025-09-02 122040" src="https://github.com/user-attachments/assets/9171730b-56bf-419e-8bc8-beba06767a44" />
<img width="750" height="751" alt="Screenshot 2025-09-02 122028" src="https://github.com/user-attachments/assets/6ab1085d-a6a6-43f5-8452-cf74d88d183b" />
<img width="926" height="576" alt="Screenshot 2025-09-02 122017" src="https://github.com/user-attachments/assets/55a92f0e-338a-4d7c-bf12-a41e6dd77e82" />
<img width="970" height="603" alt="Screenshot 2025-09-02 122009" src="https://github.com/user-attachments/assets/c6ddbf11-7494-4476-8adc-fdcc26692848" />

Contact us & Faq
![IMG-20240404-WA0010](https://github.com/user-attachments/assets/595fbbec-7ea2-4108-9911-85d2e6596c24)
![IMG-20240404-WA0009](https://github.com/user-attachments/assets/088e4eae-e580-4e36-9773-59983bb4c047)



OR run built-in PHP server:

php -S localhost:8000 -t placement-management-system
