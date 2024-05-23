# Django React JWT Authentication

This project demonstrates a full-stack web application using Django for the backend and React.js for the frontend, with JSON Web Token (JWT) authentication for securing user authentication and authorization.

## Features

- **Django Backend**: RESTful API with Django REST Framework
- **React Frontend**: User interface built with React.js
- **JWT Authentication**: Secure user authentication using JWT tokens
- **User Registration and Login**: Basic user management functionality

## Prerequisites

- Python 3.8 or higher
- Node.js and npm
- PostgreSQL (or another database supported by Django)

## Installation

### Backend Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/django-react-jwt-auth.git
   cd django-react-jwt-auth/backend






Create a virtual environment and activate it:

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install backend dependencies:


pip install -r requirements.txt
Set up environment variables:

Create a .env file in the backend directory with the following content:

env
SECRET_KEY=your_secret_key
DEBUG=True
DATABASE_URL=your_database_url
Run migrations:


python manage.py migrate
Create a superuser:


python manage.py createsuperuser
Start the backend server:

python manage.py runserver
Frontend Setup
Navigate to the frontend directory:


cd ../frontend
Install frontend dependencies:


npm install
Start the frontend development server:


npm start
The React application should automatically open in your browser at http://localhost:3000.



```django-react-jwt-auth/
├── backend/
│   ├── manage.py
│   ├── myproject/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── wsgi.py
│   │   └── ...
│   ├── requirements.txt
│   ├── .env
│   └── ...
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── services/
│   │   ├── App.js
│   │   ├── index.js
│   │   └── ...
│   ├── package.json
│   └── ...
└── README.md
```




API Endpoints
Authentication
Register: POST /api/register/
Login: POST /api/login/
User Info: GET /api/user/ (requires JWT token)
Protected Endpoints
Example Protected Endpoint: GET /api/protected/
JWT Authentication
Register: Send a POST request to /api/register/ with the user's credentials to create a new account.

Login: Send a POST request to /api/login/ with the user's credentials to receive a JWT token.

Access Protected Routes: Include the JWT token in the Authorization header as Bearer <token> for accessing protected routes.

Usage
Register a new user through the registration form in the React application.
Login with the registered user credentials to receive a JWT token.
The token will be stored in the browser's local storage and used to authenticate subsequent requests to protected endpoints.
Contributing
Contributions are welcome! Please fork this repository and submit a pull request for any features, bug fixes, or enhancements.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
Django
React
Django REST Framework
JWT


This `README.md` file provides a clear and concise guide to setting up, configuring, and running your Django with React.js project, incorporating JWT token authentication. It covers all the necessary steps for installation, configuration, and usage, ensuring that anyone can get started with the project easily.

