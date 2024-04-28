* Store Management System

The Store Management System is a Python application designed to streamline the management of a store's inventory and customer orders. It offers functionalities for both administrators and customers, allowing efficient management and improved customer experience.

** Features:

*** Admin Panel:
- Login and authentication for administrators.
- View, add, update, search, and delete products in the inventory.
- Access, manage customer information, and view order history.

*** Customer Dashboard:
- User sign up and login functionality.
- Browse available products in the store.
- Place orders, pay, view order history, and generate receipts.

** Technologies Used:

- Integrated Development Environment (IDE): Visual Studio Code
- Python
- Tkinter library (for the user interface)
- MySQL (for the database)

** Installation and Setup:

1. Clone the repository:
   `git clone https://github.com/bongchanbormey/CSA-Final-Project.git`

2. Instructions for setting up and running the application:

** Usage:

- Clone this repository and open it in the IDE of your choice, I ran this in Visual Studio Code.
- Make sure you have Tkinter library installed for the graphical user interface.
- Make sure you have MySQL server set up and running.
- Install MySQL connector using pip if you haven't (pip3 install mysql-connector-python).
- Create a database and 3 tables in MySQl.
- Build and run the application.

** MySQL Database Setup:

- Assuming that you have MySQL server installed and set up:
  + Access MySQL through the Command Prompt or Powershell (for Windows) or Terminal (for MacOS).
  + Type 'mysql -u root -p' then enter your password.
  + 'Show databases;' to see your existing databases.
  + Create a database with the name you prefer (I used 'Shop'. If you use a different database name, change it in the code too.) 
  + Create 3 tables too. Use the following command lines:

    create database Shop;

    use Shop;

    CREATE TABLE user_account(
      id INT AUTO_INCREMENT PRIMARY KEY
      username VARCHAR(100),
      password   VARCHAR(100),
      orders VARCHAR(100),
      amount VARCHAR(100),
      logged_in VARCHAR(100)
    );
    
    CREATE TABLE user_order(
      id VARCHAR(100)
      user_id VARCHAR(100),
      name   VARCHAR(100),
      quantity VARCHAR(100),
      total VARCHAR(100),
      amount VARCHAR(100)
    );
    
    CREATE TABLE products(
      id VARCHAR(100),
      name VARCHAR(100),
      type VARCHAR(100),
      price VARCHAR(100),
      stock VARCHAR(100)  
    );

** Credentials:

- Use the following credentials to access the system:
  + Username (log in as admin): admin
  + Password: 12345
