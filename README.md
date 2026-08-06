# Simple Web Application (PHP + MySQL + AJAX)

A full-stack web application built as part of the technical assessment task. The application interacts with a MySQL database to manage user records and update statuses dynamically without page reloads using AJAX.

---

## 🌐 Live Demo
You can test the deployed application directly here:
👉 **[Live Website Link](http://wedyan-portfolio.infinityfreeapp.com)**

---

## 📸 Application Screenshot
Here is a preview of the dynamic user management interface in action:

![Dynamic User Interface](app-screenshot.png)

---

## 🚀 Features & Deliverables

1. **User Interface (HTML/CSS)**: A clean, inline input form allowing users to submit their Name and Age.
2. **Database Integration (PHP & MySQL)**: Submitted data is stored directly into a MySQL database table (`users`).
3. **Data Display**: Automatically fetches and presents all database records inside a structured HTML table placed below the form.
4. **Instant Status Toggle (AJAX)**: Each record features a `Toggle` button that switches the user's status value between `0` and `1` dynamically in both the UI and MySQL database without refreshing the webpage.

---

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript (Fetch API / AJAX)
- **Backend**: PHP
- **Database**: MySQL (phpMyAdmin)
- **Hosting / Server**: InfinityFree Cloud Hosting

---

## 📁 Project Structure

- `index.php` - The main interface containing the HTML form, data rendering table, and AJAX JavaScript code.
- `db.php` - Database connection configuration file.
- `toggle_status.php` - Backend script handling asynchronous status updates received via AJAX requests.
- `README.md` - Documentation and project guide.

---

## 🗄️ Database Setup (SQL)

To replicate the database schema locally or on another host, execute the following SQL query:

```sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    age INT NOT NULL,
    status TINYINT(1) DEFAULT 0
);
