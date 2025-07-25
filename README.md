# KVBank - Java Swing Banking System

KVBank is a desktop-based banking system built using Java Swing and MySQL (via phpMyAdmin). It features a graphical user interface for managing banking operations such as login, deposits, withdrawals, transfers, and customer reports.

---

## 📁 Project Structure

```

kvbank/
│
├── Source Packages/
│   └── bank/
│       ├── account.java       // Handles account creation and updates
│       ├── balance.java       // Displays current balance
│       ├── cusreport.java     // Generates customer activity reports
│       ├── customer.java      // Customer information management
│       ├── deposit.java       // Deposit functionality
│       ├── login.java         // Login authentication
│       ├── mainmenu.java      // Main application dashboard
│       ├── transfer.java      // Transfer between accounts
│       ├── user1.java         // User role/registration management
│       └── withdraw\.java      // Withdrawal functionality
│
├── Test Packages/
├── Libraries/
└── Test Libraries/

````

---

## 💡 Features

- Secure login system for users
- Account creation and user management
- Deposit, withdraw, and transfer money between accounts
- View and manage account balances
- Generate customer reports
- User-friendly GUI using Java Swing
- MySQL (phpMyAdmin) integration for persistent storage

---

## 🛠️ Technologies Used

- **Java (Swing)** for the GUI
- **MySQL** (phpMyAdmin) for the database
- **JDBC** for database connectivity
- **NetBeans** (recommended IDE)

---

## ⚙️ Setup Instructions

### 1. Database Setup

1. Open **phpMyAdmin** and create a new database (e.g., `kvbank`).
2. Import the SQL schema (if available) or manually create the required tables:
   - `user`
   - `customer`
   - `account`
   - `deposit`
   - `withdraw`
   - `transfer`

   > If you need help generating the schema, let me know — I can help based on your code.

3. Insert some sample user data for login testing.

### 2. Java Project Setup

1. Clone or download this repository.
2. Open it in NetBeans
3. Make sure to add the MySQL JDBC driver (`mysql-connector-java-x.x.x.jar`) to your project's library:
   - In NetBeans: Right-click project > Properties > Libraries > Add JAR/Folder

4. Update your database credentials in the database connection file 

```java
Connection con;
con = DriverManager.getConnection("jdbc:mysql://localhost/kvbank", "root", "your_password");
````

5. Run `login.java` or `mainmenu.java` to launch the app.

---

## 🔐 Default Credentials (Example)

You can add sample credentials for testing:

| Username | Password | Role  |
| -------- | -------- | ----- |
| admin    | admin123 | Admin |
| user1    | pass123  | User  |

> Adjust based on your actual database values.

---

## ✅ Future Improvements

* Add database connection pooling
* Improve UI with better layout managers or JavaFX
* Add password encryption
* Implement transaction history logging

---

## 📄 License

This project is for educational use only.



