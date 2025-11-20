# Banking System – Java & MySQL (Console Application)

This project is a console-based Banking System built using Java, JDBC, and MySQL. It allows users to register, log in, open bank accounts, and perform essential banking operations securely through a command-line interface.

 # Features
 # User Management

Register with full name, email, and password

Login using email and password

Prevents duplicate user registration

# Bank Account Management

Open a bank account (generates unique account number)

Security PIN protection for account actions

Check existing account status

# Banking Operations

All financial operations use transactions (SET AUTOCOMMIT = FALSE) to ensure data integrity.

Credit Money

Debit Money (with insufficient-balance check)

Transfer Money between accounts

Check Account Balance

Each operation validates:

Correct security pin

Sufficient balance

Account existence



# Technology Stack

Programming Language	---Java

Database ---	MySQL

Database Connectivity	--- JDBC

Build Tool	--- Maven


# Database Schema (MySQL)

    User(
        full_name varchar(30),
        email varchar(30) primary key not null,
        password varchar(20)
    );


    Accounts(
    account_number bigint primary key not null,
    full_name varchar(30),
    email varchar(30) unique,
    balance decimal,
    security_pin varchar(4)
    
    );

# Result

res1.txt

res2.txt

# Contributing

Contributions, suggestions, and improvements are welcome!

Feel free to fork the repo and submit pull requests.
