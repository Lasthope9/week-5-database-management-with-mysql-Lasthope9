# week-5-database-management-with-mysql-Lasthope9

Expense Tracking Application Database
This SQL script creates the necessary tables for our expense tracking application. The database will include tables for users, expenses, categories, and payment methods. Follow the instructions below to set up your database.

Table Structure
1. Users
The users table stores information about the users of the application.

Columns:

id: Primary key, auto-incrementing integer
username: Unique username for the user
email: Unique email address for the user
password: Hashed password for the user
created_at: Timestamp when the user was created
2. Categories
The categories table stores the different expense categories.

Columns:

id: Primary key, auto-incrementing integer
name: Name of the category
description: Description of the category
3. Payment Methods
The payment_methods table stores the different payment methods used for expenses.

Columns:

id: Primary key, auto-incrementing integer
name: Name of the payment method
description: Description of the payment method
4. Expenses
The expenses table stores information about the expenses recorded by the users.

Columns:

id: Primary key, auto-incrementing integer
user_id: Foreign key referencing the users table
category_id: Foreign key referencing the categories table
payment_method_id: Foreign key referencing the payment_methods table
amount: Decimal value representing the amount of the expense
description: Description of the expense
date: Date when the expense was made
created_at: Timestamp when the expense was recorded

