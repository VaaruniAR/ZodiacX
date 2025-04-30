# ZodiacX - Authentication System

This project implements a complete login/signup system with OTP verification for the ZodiacX application. The system includes frontend components built with React and a Flask backend for authentication.

## Project Structure

```
zodiacx/
├── backend/
│   ├── app.py
│   └── requirements.txt
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Header.jsx
│   │   │   └── Footer.jsx
│   │   ├── pages/
│   │   │   ├── Home.jsx
│   │   │   ├── ZodiacQuiz.jsx
│   │   │   ├── Compatibility.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Signup.jsx
│   │   ├── styles/
│   │   │   ├── global.css
│   │   │   ├── Header.css
│   │   │   └── Auth.css
│   │   ├── App.jsx
│   │   ├── Router.jsx
│   │   └── main.jsx
```

## Frontend Setup

1. Make sure you have Node.js and npm installed.
2. Navigate to the frontend directory.
3. Install dependencies:
   ```
   npm install
   ```
4. Create the Login.jsx and Signup.jsx files in the src/pages directory.
5. Create the Auth.css file in the src/styles directory.
6. Update the Header.jsx component with the authentication handling.
7. Update the Router.jsx to include the login and signup routes.
8. Start the frontend development server:
   ```
   npm run dev
   ```

## Backend Setup

1. Make sure you have Python installed (3.7+ recommended).
2. Navigate to the backend directory.
3. Create a virtual environment:
   ```
   python -m venv venv
   ```
4. Activate the virtual environment:
   - On Windows: `venv\Scripts\activate`
   - On macOS/Linux: `source venv/bin/activate`
5. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
6. Update the email configuration in app.py:
   ```python
   app.config['MAIL_USERNAME'] = 'your_email@gmail.com'  # Replace with your email
   app.config['MAIL_PASSWORD'] = 'your_email_password'   # Replace with your email password or app password
   app.config['MAIL_DEFAULT_SENDER'] = 'your_email@gmail.com'
   ```
   
   Note: If you're using Gmail, you'll need to create an App Password instead of using your regular password. Follow these steps:
   1. Enable 2-Step Verification on your Google Account
   2. Create an App Password (Settings > Security > App Passwords)
   
7. Start the Flask server:
   ```
   python app.py
   ```

## Authentication Flow

1. **User Registration (Signup)**:
   - User enters name, email, and password
   - Backend sends OTP to the user's email
   - User enters the OTP to verify their email
   - Upon successful verification, a JWT token is generated and returned

2. **User Login**:
   - User enters email and requests OTP
   - Backend sends OTP to the user's email
   - User enters password and OTP
   - Upon successful verification, a JWT token is generated and returned

3. **Authentication State**:
   - The JWT token is stored in localStorage
   - The Header component checks for the token and verifies it with the backend
   - If the token is valid, the user's profile is displayed
   - If the token is invalid, the user is logged out

## Security Features

- Password hashing using Werkzeug's generate_password_hash
- JWT for authentication with expiration time
- Email verification using OTP (6-digit code)
- OTP expiration (10 minutes)

## Production Considerations

For a production environment, consider the following:

1. Use a proper database (PostgreSQL, MySQL, MongoDB) instead of in-memory storage
2. Set up proper environment variables for sensitive data (SECRET_KEY, email credentials)
3. Add rate limiting to prevent brute force attacks
4. Implement HTTPS
5. Add more robust error handling and logging
