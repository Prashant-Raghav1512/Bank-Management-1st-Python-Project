# Bank Management System README

This Bank Management System is a Python and MySQL based mini project that provides a simple banking interface with separate **main** and **menu** modules.\[file:1]

## Main module

The `MAIN.PY` file acts as the entry point of the project. It connects to the MySQL `bank` database, creates a `usertable` with `username` and `password`, and shows two options: Register and Login.\[file:1]

During registration, the program accepts a username and a 4-digit password, stores the details in the database, and confirms successful user creation.\[file:1] During login, it verifies the entered username and password from `usertable`; if the credentials are correct, the program loads the next module and allows the user to continue.\[file:1]

## Menu module

The `MENU.PY` file provides the main banking operations after login. It connects to the same MySQL database, enables autocommit, and displays six menu options for account and transaction handling.\[file:1]

The available options are:

* Create bank account.\[file:1]
* Transaction.\[file:1]
* Customer details.\[file:1]
* Transaction details.\[file:1]
* Delete account/details.\[file:1]
* Quit.\[file:1]

## Functions in menu

### 1\. Create bank account

This option takes account number, account holder name, phone number, address, and credit amount as input, then inserts the record into the `customerdetails` table.\[file:1]

### 2\. Transaction

This option first checks whether the entered account number exists. If valid, it gives two sub-options: withdraw amount or add amount, and then updates the balance in the `customerdetails` table.\[file:1]

### 3\. Customer details

This option searches for a customer by account number and displays the account number, account name, phone number, address, and current amount.\[file:1]

### 4\. Transaction details

This option checks the account number and then fetches transaction records from the `transactions` table. It displays fields such as date, withdrawal amount, and added amount.\[file:1]

### 5\. Delete account

This option deletes the customer record for the given account number from the database and shows a success message after deletion.\[file:1]

### 6\. Quit

This option exits the program.\[file:1]

## Program flow

1. Start the project through the main module.\[file:1]
2. Register a new user or login with an existing username and password.\[file:1]
3. After successful login, open the menu module.\[file:1]
4. Choose the required banking operation from the displayed menu.\[file:1]

## Technologies used

* Python.\[file:1]
* MySQL Connector for Python.\[file:1]
* MySQL database named `bank`.\[file:1]

## Notes

This README is prepared only from the `MAIN.PY` and `MENU.PY` portions of the project and does not include acknowledgement or other report sections.\[file:1]

