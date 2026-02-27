# 📌 HR Payroll Management System

A professional HR & Payroll Management System built using Django, Django
REST Framework, JWT Authentication, and PostgreSQL.

This project follows a monolithic architecture with modular Django apps.

------------------------------------------------------------------------

## 🚀 Tech Stack

-   Python
-   Django
-   Django REST Framework
-   Simple JWT
-   PostgreSQL

------------------------------------------------------------------------

## 🏗 Architecture

This project uses a monolithic architecture:

-   Single Django project
-   Modular internal apps
-   Single database
-   Unified deployment

### Current Modules

-   core/ → Project configuration
-   accounts/ → Custom user & employee management

### Planned Modules

-   employees/ → Employee records
-   attendance/ → Time tracking
-   payroll/ → Salary calculation
-   leave/ → Leave management
-   reports/ → Reporting & analytics

------------------------------------------------------------------------

## 👤 Custom User Model

This system uses a custom user model with:

-   Email-based authentication
-   Role-based access control
-   Admin / HR / Employee roles

### Roles

-   ADMIN
-   HR
-   EMPLOYEE

------------------------------------------------------------------------

## 🗄 Database Configuration

PostgreSQL is used as the primary database.

Create database:

    CREATE DATABASE hr_payroll_db;

Update settings.py:

    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql',
            'NAME': 'hr_payroll_db',
            'USER': 'postgres',
            'PASSWORD': 'your_password',
            'HOST': 'localhost',
            'PORT': '5432',
        }
    }

------------------------------------------------------------------------

## ⚙️ Installation (Windows PowerShell)

### 1️⃣ Clone Repository

    git clone https://github.com/your-username/hr-payroll-system.git
    cd hr-payroll-system

### 2️⃣ Create Virtual Environment

    python -m venv venv
    .\venv\Scripts\Activate.ps1

### 3️⃣ Install Dependencies

    pip install -r requirements.txt

### 4️⃣ Run Migrations

    python manage.py makemigrations
    python manage.py migrate

### 5️⃣ Create Superuser

    python manage.py createsuperuser

### 6️⃣ Run Server

    python manage.py runserver

Open in browser:

    http://127.0.0.1:8000/admin

------------------------------------------------------------------------

## 🔐 Authentication

JWT authentication is configured using Simple JWT.

-   Access Token Lifetime: 60 minutes
-   Refresh Token Lifetime: 1 day

------------------------------------------------------------------------

## 📦 Current Models

### User

-   Email (unique)
-   Role (Admin / HR / Employee)
-   Staff & permission support

### Department

-   Unique department name

### Employee

-   Linked to User (One-to-One)
-   Department
-   Designation
-   Base salary
-   Joining date
-   Active status

------------------------------------------------------------------------

## 🎯 Future Improvements

-   Payroll processing module
-   Attendance tracking
-   Leave management system
-   Role-based API permissions
-   Salary slip generation (PDF)
-   Reporting dashboard
-   API documentation

------------------------------------------------------------------------

## 📌 Project Status

🟢 Foundation Completed\
🟡 Core HR modules in progress\
🔜 Payroll engine implementation next

------------------------------------------------------------------------

## 👨‍💻 Author

Your Name\
GitHub: https://github.com/your-username
