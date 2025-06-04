# 🏥 Hospital Staff Management System

## 🧾 Abstract
This JavaFX-based application efficiently manages hospital staff operations using a Model-View-Controller (MVC) architecture. It supports role-based access for Admin, Manager, and Staff users to streamline user-specific functionalities. Admins have full control over staff and department data, Managers can manage staff profiles and reports, and Staff can view their schedules and tasks. The backend uses MySQL to securely store and manage all data, with features like password hashing and robust error handling to ensure security and reliability.

---

## 🚀 Key Features

- 🗃️ **Database**: MySQL backend with tables for Registered Users, Staff Profiles, and Departments
- 🖥️ **Frontend**: JavaFX GUI for user-friendly interaction
- 🔐 **Security**:
  - Password hashing with BCrypt and static salt
  - Role-based access control (Admin, Manager, Staff)
- ⚙️ **Functionality**:
  - Login authentication with role-specific dashboards
  - CRUD operations on staff and departments (restricted by role)
  - Progress bar during loading, personalized welcome messages
- 📝 **Logging**:
  - Severity-based logging for efficient debugging and error tracking

---

## 🛠️ System Architecture & Workflow

### 1. MVC Pattern
- **Model**: Manages data and database interactions
- **View**: JavaFX FXML files for UI layout (login, dashboard, staff, department views)
- **Controller**: Handles user interactions, business logic, and navigation

### 2. User Roles and Permissions
- **Admin**: Full access to all data and system settings
- **Manager**: Manage staff profiles, allocate tasks, view reports (no department management)
- **Staff**: View own schedules and assigned tasks only

### 3. Security Features
- Passwords are hashed before storage using BCrypt with a static salt
- Secure database credentials stored externally in config files
- Role-based access enforced throughout the application

### 4. CRUD Operations
- Admins and Managers can Create, Read, Update, Delete staff records (with restrictions)
- Only Admins can manage departments fully
- Staff can only view their own information

---

## 📸 Visual Overview

- Splash screen with progress bar
- Role-based login screen
- Dashboard with navigation buttons and personalized welcome
- Staff management interface with table views and forms
- Department management UI with add/update/delete functionality
- Logging and alerts for smooth user experience

---

## 💻 Deployment

- Run the `Main.java` file to launch the application.
- Requires JavaFX and MySQL database setup (configurable via `config.properties`).
- Compatible with Java 8+ and MySQL Server.

---

## 👨‍💻 Authors

- **Padmavathi Vyshnavi Madarampalli** – Data processing, UI design, and role management  
- **Satya** – Backend development, database design, and security implementation  

Master’s in Information Technology and Management – ILLINOIS INSTITUTE OF TECHNOLOGY

---

## 📚 References

1. JavaFX official documentation  
2. MySQL official documentation  
3. BCrypt hashing algorithm for password security  
4. MVC architectural pattern best practices  

---

## 🔮 Future Enhancements

- Integrate reporting dashboards for managers with analytics  
- Implement machine learning models for predictive staffing needs  
- Develop mobile-friendly versions or web app integration  
- Add multi-factor authentication for enhanced security  

---

## 📄 License

This project is licensed under the MIT License – see the `LICENSE` file for details.

