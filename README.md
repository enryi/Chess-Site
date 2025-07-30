# Chess Site Installation Guide

This guide will walk you step-by-step through installing the chess site, from setting up the environment to loading the SQL database.

---

## 1. Prerequisites

To run the site, you need:

- A **web server** with PHP support (version 7.2 or higher)
- A **MySQL or MariaDB database**
- **phpMyAdmin** or another tool to manage the database
- A properly configured PHP interpreter

---

## 2. Installing PHP, MySQL, and phpMyAdmin

### On Windows

The easiest way to install everything is to use a package like **XAMPP**, which includes Apache, PHP, MySQL, and phpMyAdmin:

- Download XAMPP from [https://www.apachefriends.org/index.html](https://www.apachefriends.org/index.html)
- Run the installer and follow the instructions
- Start Apache and MySQL via the XAMPP Control Panel
- Access phpMyAdmin by opening your browser at: `http://localhost/phpmyadmin`

### On Linux (Ubuntu/Debian)

You can install the LAMP stack and phpMyAdmin using the terminal:
