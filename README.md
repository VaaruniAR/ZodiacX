# ZodiacX - Explore Your Cosmic Connection

ZodiacX is an interactive web application that helps users discover their zodiac sign, explore astrological compatibility, and engage with cosmic content. This React-based application features a beautiful cosmic-themed UI with authentication functionality.

![ZodiacX Screenshot](Screenshot 2025-04-30 at 8.42.53 AM.png)

## 🌟 Features

- **User Authentication**: Signup and login with profile management
- **Know Your Zodiac**: Interactive quiz to discover your zodiac sign
- **Compatibility Check**: Explore astrological compatibility between signs
- **Responsive Design**: Beautiful cosmic-themed UI that works on all devices
- **Persistent User Sessions**: User authentication persists between sessions

## 🚀 Installation

### Prerequisites
- Node.js (v14.0.0 or later)
- npm (v6.0.0 or later)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/zodiacx.git
   cd zodiacx
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to http://localhost:5173 (or the port shown in your terminal)

## 📂 Project Structure

```
zodiacx/
├── src/
│   ├── components/            # Reusable UI components
│   │   ├── Header.jsx         # Navigation header with auth
│   │   └── Footer.jsx         # Page footer
│   ├── pages/                 # Page components
│   │   ├── Home.jsx           # Landing page
│   │   ├── Login.jsx          # Authentication page
│   │   ├── Signup.jsx         # Registration page
│   │   ├── ZodiacQuiz.jsx     # Quiz to find zodiac sign
│   │   └── Compatibility.jsx  # Compatibility checker
│   ├── services/              # Business logic
│   │   └── localAuthService.js # Authentication service
│   ├── styles/                # CSS styles
│   │   ├── global.css         # Global styles
│   │   ├── Header.css         # Header-specific styles
│   │   └── Auth.css           # Authentication page styles
│   ├── App.jsx                # Main app component
│   ├── Router.jsx             # Application routes
│   └── main.jsx               # Entry point
├── public/                    # Static assets
├── package.json               # Project dependencies
└── vite.config.js             # Vite configuration
```

## 🔐 Authentication System

ZodiacX uses a localStorage-based authentication system that allows for:

- **User Registration**: Create a new account with name, email, and password
- **User Login**: Authenticate with email and password
- **Profile Display**: Shows user info in the header when logged in
- **Logout**: Available by clicking on the user's profile name

### Default Test User
- **Email**: test@example.com
- **Password**: password123

## 🔮 Pages and Features

### Home Page
The landing page introduces users to ZodiacX with information about the 12 zodiac signs, categorized by their elements (Fire, Earth, Air, Water).

### Know Your Zodiac Quiz
An interactive quiz that helps users discover their zodiac sign based on their personality traits and preferences.

### Compatibility Checker
Users can select two zodiac signs to check their astrological compatibility across different aspects like love, friendship, and communication.

### Login/Signup Pages
Cosmic-themed authentication pages with form validation and error handling.

## 💻 Development

### Adding New Pages
1. Create a new component in the `src/pages` directory
2. Add the route in `Router.jsx`
3. Link to it from the navigation if needed

### Styling Guidelines
- Follow the cosmic theme with gradients and space-like elements
- Use variables defined in `global.css` for consistent colors
- Ensure responsive design for all screen sizes

## 📱 Responsive Design

ZodiacX is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones

The UI adapts automatically using media queries to provide the best experience on any device.

## 🛠️ Technologies Used

- **React**: UI library for building the interface
- **React Router**: For navigation and routing
- **Vite**: Build tool and development server
- **CSS**: Custom styling with responsive design
- **localStorage**: For persisting authentication state

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- Zodiac sign information and compatibility data from [Astrology.com](https://www.astrology.com)
- Star background animation inspired by [Starry Night codepen](https://codepen.io/sarazond/pen/LYGbwj)
- Icons from [Remix Icon](https://remixicon.com/)

---

Created with ❤️ and cosmic energy by Vaaruni
