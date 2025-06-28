# Web-User-Registration-System 🌐

This project was developed as part of the **Web Based Information Systems** course (IS333 - Spring 2025), Faculty of Computers and Artificial Intelligence, Cairo University.

It implements a user registration web page following the MVC architecture, with robust validation and third-party API integration.

---

## ✨ Features

- User registration form capturing:
  - Full name
  - Username
  - Phone
  - WhatsApp number (with validation via external API)
  - Address
  - Email
  - Password and confirmation
  - User profile image upload
- Client-side validation for:
  - Mandatory fields
  - Email format
  - Password strength (min 8 chars, at least 1 number, 1 special character)
  - Password match
- Server-side validation:
  - AJAX check for unique usernames
- Integration with WhatsApp Number Validator API via RapidAPI
- Image upload and storage on the server
- Custom header and footer integrated into the registration page
- MySQL database to store user data

---

## 💻 Technologies Used

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** PHP, AJAX
- **Database:** MySQL
- **API Integration:** RapidAPI (WhatsApp Number Validator)

---

## 🗂️ Project Structure (MVC)
```
/project-root
│── /app
│   ├── /controllers
│   │   ├── UserController.php      # Handles registration logic & API requests
│   │   ├── UploadController.php    # Handles image uploads
│   │
│   ├── /models
│   │   ├── DB_ops.php                  # Database connection class
│   │
│   ├── /views
│   │   ├── header.php              # Header design
│   │   ├── footer.php              # Footer design
│   │   ├── index.php               # Main registration page
│   │
│── /public
│   ├── /css
│   │   ├── styles.css              # Stylesheet
│   │
│   ├── /js
│   │   ├── validations.js          # Client-side form validation
│   │   ├── api_ops.js              # JavaScript for WhatsApp API calls
│   │
│   ├── /uploads                    # Directory for storing uploaded images
│
│── /config
│   ├── config.php                  # Database credentials & app settings
│
│── /database
│   ├── user_management.sql                   # Backup of your database
│
│── .htaccess                         # URL routing (optional)
│── team_members.txt                  # Team members' names and IDs
│── README.md                         # Project instructions
```


---

## 🛠️ How to Restore Database

1. Open [phpMyAdmin](http://localhost/phpmyadmin)
2. Click **Import** tab
3. Choose `user_management.sql`
4. Click **Go**

---

## 👥 Team Members

This project was developed by a team of **6 students** as part of the Web Based Information Systems course.

- Israa Mohamed
- Amany Mohamed
- Joseph Sameh
- Youssef Joseph
- Nour Ahmed
- Jonathan Mokhles


- **Frontend Developer (HTML/CSS)**
    - Designed `index.php`, `header.php`, and `footer.php`
- **Frontend Developer (JavaScript)**
    - Developed `validations.js` for client-side validation
    - Developed `api_ops.js` for API integration
- **Backend Developer (PHP - Controllers)**
    - Developed `UserController.php` for registration logic
    - Implemented AJAX username validation
- **Backend Developer (PHP - Models)**
    - Developed `DB_ops.php` for database operations
- **Image Handling & Deployment**
    - Developed `UploadController.php` for handling image uploads
    - Managed deployment and database backup

---
