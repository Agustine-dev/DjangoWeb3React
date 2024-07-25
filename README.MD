---
# Web3 Project: Django and React Authentication with JWT and HTTP-Only Cookies

This project implements a user authentication system using Django and React. It includes user registration, login, logout, and fetching user data. Authentication is handled using JWT (JSON Web Tokens) and HTTP-only cookies for improved security. The application's frontend is styled using Bootstrap.

## Features

- **User Registration**: Users can create an account.
- **User Login**: Users can log in to their account.
- **User Logout**: Users can log out of their account.
- **Fetch User Data**: Authenticated users can fetch their profile data.
- **JWT Authentication**: JSON Web Tokens are used for secure authentication.
- **HTTP-Only Cookies**: JWT tokens are stored in HTTP-only cookies to prevent XSS attacks.
- **Frontend Styling**: The frontend is styled using Bootstrap.

## Project Structure

```plaintext
root
├── client      # React frontend
└── server      # Django backend
```

## Getting Started

### Prerequisites

- Node.js and npm installed
- Python and pip installed
- Django installed
- A virtual environment for Python

### Setup

#### Backend (Django)

1. **Navigate to the server directory**:
    ```sh
    cd server
    ```

2. **Create and activate a virtual environment**:
    ```sh
    python -m venv venv
    venv\Scripts\activate  # On Windows
    source venv/bin/activate  # On macOS/Linux
    ```

3. **Install the dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

4. **Run migrations**:
    ```sh
    python manage.py migrate
    ```

5. **Run the Django development server**:
    ```sh
    python manage.py runserver
    ```

#### Frontend (React)

1. **Navigate to the client directory**:
    ```sh
    cd client
    ```

2. **Install the dependencies**:
    ```sh
    npm install
    ```

3. **Start the React development server**:
    ```sh
    npm start
    ```

### Environment Variables

Create a `.env` file in the `server` directory with the following variables:

```plaintext
SECRET_KEY=your_secret_key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
CORS_ALLOWED_ORIGINS=http://localhost:3000
```

Create a `.env` file in the `client` directory with the following variables:

```plaintext
REACT_APP_API_URL=http://localhost:8000
```

## Usage

- **User Registration**: Visit the registration page and fill out the form to create a new account.
- **User Login**: Visit the login page and enter your credentials to log in.
- **User Logout**: Click the logout button to end your session.
- **Fetch User Data**: After logging in, visit the profile page to see your user data.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you would like to contribute to the project.

## License

This project is licensed under the MIT License.
---