# ♟️ Chess Website Installation Guide

Welcome to my Chess Website! This guide will walk you through the steps needed to install and run the project locally.

---

## 📦 Requirements

Before getting started, ensure you have the following installed:

- [PHP (>= 7.4)](https://www.php.net/downloads)
- [MySQL / MariaDB](https://dev.mysql.com/downloads/mysql/) (used for database)
- [phpMyAdmin](https://www.phpmyadmin.net/downloads/) (optional, but recommended for managing the database)
- [Apache](https://httpd.apache.org/download.cgi) or another local server like [XAMPP](https://www.apachefriends.org/index.html)

> 💡 If you're new to web servers, we recommend installing **XAMPP** as it includes PHP, MySQL, and Apache in one package.

---

## 🚀 Installation Steps

### 1. Clone or Download the Repository

```bash
git clone https://github.com/enryi/Chess-Site.git
```

Or download and extract the ZIP file manually.

Place the folder into your web server's root directory:
- **XAMPP**: `C:\xampp\htdocs\`
- **Linux Apache**: `/var/www/html/`

---

### 2. Set Up the Database

#### Option A: Using phpMyAdmin

1. Start your Apache and MySQL server.
2. Open [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
3. Create a new database (e.g., `chess_db`).
4. Import the SQL file:
   - Click the database name.
   - Go to the **Import** tab.
   - Choose the file: `database.sql` (located in the project folder).
   - Click **Go**.

#### Option B: Using the MySQL Command Line

```bash
mysql -u root -p
```

```sql
CREATE DATABASE chess_db;
USE chess_db;
SOURCE /path/to/database.sql;
```

---

### 3. Configure Database Connection

Open the configuration file, usually located at:

```
/config/database.php
```

Edit the following lines to match your setup:

```php
$host = 'localhost';
$db   = 'chess_db';
$user = 'root';
$pass = ''; // default password is empty in XAMPP
```

---

### 4. Start the Server

If using XAMPP or another local server:
1. Start Apache and MySQL via the XAMPP control panel.
2. Navigate to your browser and go to:

```
http://localhost/chess-website
```

You should now see the homepage of the chess site.

---

## 🛠 Troubleshooting

- If the site shows a blank page, make sure `display_errors` is enabled in your `php.ini` file.
- Ensure your database credentials are correct.
- If the database import fails, double-check the SQL file and database name.

---

## 📚 Helpful Links

- [Download PHP](https://www.php.net/downloads)
- [Download MySQL](https://dev.mysql.com/downloads/mysql/)
- [Download phpMyAdmin](https://www.phpmyadmin.net/downloads/)
- [Download XAMPP (Recommended)](https://www.apachefriends.org/index.html)

---

## ❤️ Credits

Created by [enryi]. Feel free to fork, contribute, or report issues.

---
