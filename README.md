# 🚪 Visitor Management System

A containerized **Visitor Management System** built using **PHP, MySQL, Docker, and Docker Compose**.

The application is designed for security personnel to record and manage visitor/customer information such as name, mobile number, email, contact person, reason for visit, and visit timestamp.

---

## 📌 Project Overview

The Visitor Management System provides a simple web-based interface for security personnel to maintain visitor records.

The system allows users to:

- Add new visitors
- View all visitor records
- Filter visitors based on reason for visit
- Automatically capture visit timestamps
- Store visitor information in a MySQL database

The complete application is containerized using **Docker** and can be deployed using **Docker Compose**.

---

## ✨ Features

### 👤 Add New Visitor

Security personnel can enter:

- Visitor Name
- Mobile Number
- Email Address
- Contact Person Name
- Reason for Visit

Available visit reasons:

- Purchasing
- Enquiry
- Dispute
- Meeting
- Presentation
- Others

The visit timestamp is automatically recorded.

### 📋 View All Visitors

The application provides a page to display all visitor records stored in the MySQL database.

### 🔎 Filter Visitors

Visitors can be filtered based on their reason for visiting.

### 🗄️ MySQL Database

All visitor information is stored in a MySQL database.

### 🐳 Containerized Application

The application runs using separate Docker containers for:

- PHP/Apache application
- MySQL database

Docker Compose manages both containers.

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| PHP 8.0 | Backend application |
| Apache | Web server |
| MySQL 8.0 | Database |
| PDO | MySQL database connectivity |
| Docker | Containerization |
| Docker Compose | Multi-container management |
| Amazon Linux 2023 | Server operating system |
| AWS EC2 | Cloud deployment |
| HTML | Frontend |

---

# 📁 Project Structure

```text
visitor-management-app/
│
├── app/
│   ├── db.php
│   ├── index.php
│   ├── add_visitor.php
│   ├── fetch_all.php
│   ├── fetch_by_reason.php
│   └── Dockerfile
│
├── mysql/
│   ├── Dockerfile
│   └── init.sql
│
├── docker-compose.yml
│
└── README.md
