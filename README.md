# Banking-Management-System
Overview

The Banking Management System is a Python-based project designed to efficiently manage user accounts across multiple banks, including SBI, PMB, and Kotak. It offers a comprehensive suite of functionalities such as user registration, secure login, fund withdrawal, deposits, balance inquiries, and account closure. This system ensures data persistence through file handling and incorporates password hashing for enhanced security.

Key Features

1. User Authentication

Registration: Enables users to create accounts with unique usernames and passwords.

Secure Login: Validates user credentials during login, ensuring restricted access to accounts.

Password Hashing: Implements SHA-256 hashing to securely store user passwords.

2. Multi-User Support

Accommodates up to 5 unique user registrations.

Ensures data integrity and user-specific account management.

3. Banking Services

Withdrawals: Allows users to securely withdraw funds if sufficient balance exists.

Deposits: Facilitates fund deposits to user accounts.

Balance Inquiries: Enables users to view current account balances.

Account Closure: Allows users to close accounts and remove their data permanently.

4. Multi-Bank Functionality

Supports account management for SBI, PMB, and Kotak, offering users the flexibility to choose their preferred bank.

Project Architecture

users.txt: Stores hashed user credentials.

accounts.txt: Maintains account details, including account numbers, names, and balances.

main.py: Serves as the main script containing core functionalities and user interaction workflows.


Functional Modules

User Registration

Users can register by providing a unique username and password.

The system securely stores credentials using SHA-256 hashing.

Registration is limited to a maximum of 5 users to ensure system manageability.

Secure Login

Validates user credentials during the login process.

Prevents unauthorized access to accounts.

Banking Operations

Withdrawals: Deducts user-specified amounts from account balances, subject to available funds.

Deposits: Adds funds to user accounts, updating the balance instantly.

Balance Check: Displays current account balances for users.

Account Closure: Permanently deletes account data upon user request.

Multi-Bank Support

Users can select from supported banks (SBI, PMB, Kotak) during registration and account management.

Technical Requirements

Python 3.x

Standard Python Libraries: os, hashlib

Code Highlights

hash_password(password)

Implements SHA-256 hashing for secure password storage, enhancing user data protection.

user_info()

Manages user registration, ensuring unique usernames and adherence to the user limit.

login()

Facilitates user authentication by verifying credentials against stored data.

Banks Class

Encapsulates core banking functionalities, including account creation, fund transactions, balance inquiries, and account closure.

Future Prospects

Transition to database integration for scalable data management.

Implementation of multi-factor authentication for heightened security.

Expansion to support additional banks and advanced services such as loans and fixed deposits.

Acknowledgments

This project was developed as an educational initiative to demonstrate file handling, object-oriented programming, and secure user management using Python. It reflects foundational concepts essential for real-world banking applications.

License

This project is distributed under the MIT License. You are free to use, modify, and distribute it, subject to the terms of the license.
