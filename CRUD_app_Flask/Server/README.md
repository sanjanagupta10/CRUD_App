# Flask CRUD App with MySQL or PostgreSQL

## Description

This is a simple Flask CRUD application that manages a list of books stored in a database. The app supports both **MySQL** and **PostgreSQL**, allowing users to create, read, update, and delete books. Depending on your database preference, the app will automatically direct you to use either **app_mysql.py** (for MySQL) or **app.py** (for PostgreSQL).

## Technologies Used

- Flask (Backend Framework)
- Flask-CORS (Cross-Origin Resource Sharing)
- If using **MySQL**:
    - mysql-connector-python (MySQL driver for Python)
- If using **PostgreSQL**:
    - psycopg2 (PostgreSQL driver for Python)
    - psycopg2-binary

## Prerequisites

Ensure the following are installed on your system:
- Python 3.x
- MySQL or PostgreSQL
- pip (Python package manager)

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   
# DATABASE SETUP-

**create a database**
CREATE DATABASE demo_flask;

**Create the book table in the demo_flask database:**
CREATE TABLE book (
    id INT AUTO_INCREMENT PRIMARY KEY,
    publisher VARCHAR(255),
    name VARCHAR(255),
    date DATE
);

## Configure the database in your code: In the respective Python file (app_mysql.py for MySQL or app.py for PostgreSQL), update the db_config object with your database credentials:

db_config = {
    'host': 'localhost',
    'user': '<your-username>',  # Use your MySQL or PostgreSQL username
    'password': '<your-password>',  # Your MySQL or PostgreSQL password
    'dbname': 'demo_flask'  # The database name
}

# Go to the Server Directory If you're not in Server Directory
```bash
cd Server
```
# Run the Application:

- **For MySQL:**
    - python app_mysql.py

- **For PostgreSQL:**
    - python app.py

## Usage
Once the app is running, you can interact with it through your browser at http://localhost:5000.

**Create** a book: Use a form to add a book to the database.
**Read:** View the list of books.
**Update:** Edit the details of a book.
**Delete:** Remove a book from the database.

