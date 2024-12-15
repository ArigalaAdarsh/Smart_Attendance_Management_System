# Smart Attendance Project

## Overview

The Smart Attendance project is a web-based system developed to simplify the attendance tracking process for teachers and provide students with a convenient way to view their attendance statistics. The project incorporates HTML, CSS, Bootstrap, JavaScript, Flask, and Microsoft SQL Server to create a responsive and dynamic attendance management system.

## Features

### Teacher Module

- **Mark Attendance:**
  - Teachers can mark attendance for students in real-time through an intuitive web interface.
  
- **View Attendance Records:**
  - Teachers can view and manage attendance records for individual students or entire classes.

### Student Module

- **View Attendance Statistics:**
  - Students can log in to view their attendance statistics, including the number of classes attended and absent.
  
- **Interactive Pie Chart:**
  - An interactive pie chart visually represents the attendance statistics for better comprehension.

## Technologies Used

- **Frontend:**
  - HTML
  - CSS
  - Bootstrap
  - JavaScript

- **Backend:**
  - Flask (Python Web Framework)

- **Database:**
  - Microsoft SQL Server

## Setup Instructions

1. Clone the repository:

    ```bash
    git clone https://github.com/ArigalaAdarsh/Smart_Attendance_Management_System.git
    ```

2. Set up the database:
   - Create a new database in Microsoft SQL Server.
   - Configure the database connection in the Flask app. Set the following environment variables in your app:

    ```python
    # Database Configuration
    server = ''  # Add your SQL Server details (e.g., localhost or remote server address)
    database = ''  # Add your database name
    username = ''  # Add your SQL Server username
    password = ''  # Add your SQL Server password
    ```

3. Configure the email service:
   - If you want to send email notifications (for example, attendance reminders), set the following environment variables:

    ```python
    # Email Configuration
    email_address = os.environ.get("EMAIL_ADDRESS", " ")  # Add your Email address
    email_password = " "  # Add your Email App Password
    smtp_server = "smtp.gmail.com"  # SMTP server for Gmail
    smtp_port = 587  # SMTP port for Gmail
    ```

4. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

5. Run the Flask app:

    ```bash
    python app.py
    ```

6. Open the application in your web browser:

    ```
    http://localhost:5000
    ```

## Contributing

If you'd like to contribute to the project, please fork the repository and create a pull request. We welcome your contributions!

---

*Note: Make sure to replace the placeholder values for your SQL Server and email configuration with the appropriate credentials for your setup.*
