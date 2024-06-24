# Employee Management System

## Overview
The Employee Management System is a simple console-based application for managing employee records using a MySQL database.

## Features
1. **Add Employee**: Add a new employee to the database.
2. **Remove Employee**: Remove an existing employee from the database.
3. **Promote Employee**: Increase an employee's salary.
4. **Display Employees**: Show all employees in the database.
5. **Exit**: Exit the application.

## Prerequisites
- Python 3.x
- MySQL Server
- `mysql-connector-python` library

## Installation
1. Install Python 3.x from [python.org](https://www.python.org/downloads/).
2. Install MySQL Server from [mysql.com](https://dev.mysql.com/downloads/installer/).
3. Install the MySQL Connector library:
   ```bash
   pip install mysql-connector-python
   ```

4. Set up the database:
   - Create a database named `emp`.
   - Create a table named `employees`:
     ```sql
     CREATE TABLE employees (
         id INT PRIMARY KEY,
         name VARCHAR(100),
         position VARCHAR(100),
         salary DECIMAL(10, 2)
     );
     ```

## Configuration
Update the database connection details in the script if necessary:
```python
con = mysql.connector.connect(
    host="localhost",
    user="root",
    password="root",
    database="emp"
)
```

## Usage
Run the script:
```bash
python employee_management.py
```

Follow the menu options to add, remove, promote, or display employees.
