# 🏥 Hospital Management System

A simple **console-based Java application** that manages hospital operations like patient registration, doctor details, and appointment booking using **MySQL** and **JDBC**.

---

## 📌 Features

### 👨‍⚕️ Patient Management
- Add new patients
- View all registered patients
- Check if a patient exists by ID

### 🩺 Doctor Management
- View all available doctors
- Check if a doctor exists by ID

### 📅 Appointment Booking
- Book appointments for patients with doctors
- Prevent double-booking on the same date
- Validate patient and doctor availability

---

## 🛠️ Technologies Used

- **Java** (JDK 8 or higher)
- **JDBC** (Java Database Connectivity)
- **MySQL** (Relational Database)
- IDE: IntelliJ IDEA / Eclipse (optional)
- MySQL Workbench (for DB setup)

---

## 🧱 Database Schema

### `patients` Table
| Column      | Type         | Description         |
|-------------|--------------|---------------------|
| id          | INT (PK)     | Patient ID          |
| name        | VARCHAR      | Patient Name        |
| age         | INT          | Age                 |
| gender      | VARCHAR      | Gender              |

### `doctors` Table
| Column      | Type         | Description         |
|-------------|--------------|---------------------|
| id          | INT (PK)     | Doctor ID           |
| name        | VARCHAR      | Doctor Name         |
| specialization | VARCHAR   | Specialization      |

### `appointments` Table
| Column        | Type         | Description             |
|---------------|--------------|-------------------------|
| id            | INT (PK)     | Appointment ID          |
| patient_id    | INT (FK)     | Refers `patients(id)`   |
| doctor_id     | INT (FK)     | Refers `doctors(id)`    |
| appointment_day | DATE       | Appointment Date        |

---

## 🚀 How to Run

1. **Clone the repository**
   git clone https://github.com/your-username/hospital-management-system.git
   cd hospital-management-system
