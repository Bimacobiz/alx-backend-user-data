# 0x02-Session Authentication

## Overview

This project focuses on implementing session-based authentication in a Flask application. Session authentication is a common method used to manage user authentication in web applications. It involves storing user session data on the server and providing a session identifier to the client, usually in the form of a cookie.

In this project, we implement session authentication using Flask's built-in session management capabilities. Users can log in, log out, and access protected routes based on their authentication status.

## Features

- User registration: New users can sign up for an account by providing a username and password.
- User login: Registered users can log in using their credentials.
- Session management: User sessions are managed using Flask's session functionality.
- Access control: Certain routes are protected and can only be accessed by authenticated users.

## Setup

1. **Clone the Repository**: 
    ```
    git clone <repository-url>
    ```

2. **Install Dependencies**: 
    ```
    pip install -r requirements.txt
    ```

3. **Run the Application**: 
    ```
    API_HOST=0.0.0.0 API_PORT=5000 python3 -m api.v1.app
    ```

4. **Access the Application**: Open a web browser and navigate to `http://localhost:5000` to access the application.

## Usage

1. **User Registration**: 
    - Navigate to the registration page.
    - Enter a username and password.
    - Click the "Register" button.

2. **User Login**: 
    - Navigate to the login page.
    - Enter your registered username and password.
    - Click the "Login" button.

3. **Access Protected Routes**: 
    - After logging in, you can access protected routes such as the user dashboard.

4. **User Logout**: 
    - Click the "Logout" button to log out of your session.

## Project Structure

- `api/`: Contains the Flask application code.
    - `v1/`: Version 1 of the API.
        - `app.py`: Main Flask application file.
        - `views/`: Contains view functions for handling different routes.
        - `models/`: Contains data models for the application.
- `tests/`: Contains unit tests for the application.
- `requirements.txt`: List of Python dependencies required for the project.
- `LICENSE`: License file.
- `README.md`: This file.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

