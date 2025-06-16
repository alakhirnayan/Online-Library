
````markdown
# 📚 Online Library Management System

A simple web-based **Library Management System** developed in PHP and MySQL that allows users (students/faculty) to request, issue, return books, and manage their profiles. Admins can manage book records, user accounts, and requests.

---

## 💡 Features

### 👨‍🏫 Admin Panel
- Login & logout for administrators
- View/add/edit/delete books
- View all members and their profiles
- Handle book issue and return records
- Respond to book requests

### 👤 Member Panel (Students / Faculty)
- Login & logout system
- View and edit personal profile
- Search for books
- Request books
- View issued/returned book history

### 🌐 General
- Clean interface with navigation
- Separated codebase for **admin** and **member** controllers
- Fully styled using custom CSS
- Relational database structure (MySQL)

---

## 🛠️ Technologies Used

- **Frontend**: HTML, CSS
- **Backend**: PHP
- **Database**: MySQL
- **Web Server**: Apache (Recommended via XAMPP/LAMP)

---

## 📁 Project Structure

```bash
controller/
├── admin/         # Admin-side logic & views
├── member/        # Member-side logic & views
├── adminLogin.php
├── facultyLogin.php
├── studentLogin.php
├── register.php
├── dbConfig.php
├── ...
public/
├── css/           # All CSS files (register.css, navigation.css, etc.)
sql/
├── libsystem.sql  # MySQL database structure and initial data
index.php          # Entry point
````

---

## ⚙️ Installation Instructions

### 1️⃣ Requirements

* PHP 5.5+ (PHP 7+ recommended)
* MySQL 5.x or compatible
* Apache web server
* Browser (Chrome, Firefox, etc.)

**Recommended Stack**: [XAMPP](https://www.apachefriends.org/index.html) (Windows/macOS/Linux)

---

### 2️⃣ Setup Steps

#### 🔸 Step 1: Clone the Repository

```bash
git clone https://github.com/alakhirnayan/Online-Library.git
```

> Or [download the ZIP](https://github.com/alakhirnayan/Online-Library/archive/refs/heads/main.zip) and extract it.

#### 🔸 Step 2: Move Files to Web Server Directory

Place the extracted folder into your server directory:

* For **XAMPP**: `C:\xampp\htdocs\online-library-system`
* For **LAMP**: `/var/www/html/online-library-system`

#### 🔸 Step 3: Import Database

1. Start **XAMPP** (or your stack).
2. Open [phpMyAdmin](http://localhost/phpmyadmin).
3. Create a new database named:

```text
libsystem
```

4. Import the `libsystem.sql` file found in the `sql/` folder.

#### 🔸 Step 4: Configure Database Connection

Edit the `controller/dbConfig.php` file if your DB credentials are different:

```php
$host = "localhost";
$user = "root";         // Default for XAMPP
$password = "";         // Default for XAMPP
$database = "libsystem";
```

#### 🔸 Step 5: Run the Project

Go to your browser and open:

```text
http://localhost/online-library-system/index.php
```

Use the default admin login:

```
Username: akhir
Password: 108424aa
```

---

## 📝 Developer Info

This project was created by **Al-Akhir Nayan**.

If you have questions or want to collaborate, feel free to contact me at:

📧 **[asquiren@gmail.com](mailto:asquiren@gmail.com)**

---

## 📌 Notes

* Some CSS files may need minor corrections (`rgeba(...)` → `rgba(...)`).
* You can extend this system with pagination, AJAX interactions, and validation.
* Add `.htaccess` routing or adopt a PHP framework (like Laravel) for production.

---

## ✅ License

This project is open-source and free to use for educational or non-commercial purposes.

```


