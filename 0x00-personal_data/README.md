# 0x00-personal_data

## Overview
The "0x00-personal_data" repository contains code and resources related to handling and protecting personal data in software applications. It focuses on implementing best practices and security measures to ensure the privacy and security of user information.

## Resources
Read or watch:
- [What Is PII, non-PII, and Personal Data?](https://digitalguardian.com/blog/what-personally-identifiable-information-pii)
- [Logging Documentation](https://docs.python.org/3/library/logging.html)
- [bcrypt Package](https://pypi.org/project/bcrypt/)

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
- Examples of Personally Identifiable Information (PII)
- How to implement a log filter that will obfuscate PII fields
- How to encrypt a password and check the validity of an input password
- How to authenticate to a database using environment variables

## Requirements
- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using Python3 (version 3.7)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/env python3`
- A README.md file, at the root of the folder of the project, is mandatory
- Your code should use the PEP8 style (version 2.5)
- All your files must be executable
- The length of your files will be tested using `wc`
- All your modules should have documentation (`python3 -c 'print(__import__("my_module").__doc__)'`)
- All your classes should have documentation (`python3 -c 'print(__import__("my_module").MyClass.__doc__)'`)
- All your functions (inside and outside a class) should have documentation (`python3 -c 'print(__import__("my_module").my_function.__doc__)'` and `python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'`)
- A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)
- All your functions should be type annotated

## Tasks
### 0. Regex-ing (mandatory)
Write a function called `filter_datum` that returns the log message obfuscated.

- Arguments:
  - `fields`: a list of strings representing all fields to obfuscate
  - `redaction`: a string representing by what the field will be obfuscated
  - `message`: a string representing the log line
  - `separator`: a string representing by which character is separating all fields in the log line (message)

### 1. Log formatter (mandatory)
Update the `RedactingFormatter` class to accept a list of strings `fields` constructor argument.

### 2. Create logger (mandatory)
Implement a `get_logger` function that takes no arguments and returns a `logging.Logger` object.

### 3. Connect to secure database (mandatory)
Implement a `get_db` function that returns a connector to the database.

### 4. Read and filter data (mandatory)
Implement a `main` function that retrieves all rows in the users table and displays each row under a filtered format.

### 5. Encrypting passwords (mandatory)
Implement a `hash_password` function that expects one string argument `password` and returns a salted, hashed password.

### 6. Check valid password (mandatory)
Implement an `is_valid` function that expects 2 arguments and returns a boolean.


