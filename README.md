# ZodiacX - Cosmic Connections App

A React application that allows users to explore zodiac signs, discover their zodiac personality through a quiz, and check compatibility between zodiac signs.

## Features

- **Home Page**: Gallery of all zodiac signs with beautiful UI
- **Zodiac Quiz**: Personalized quiz to discover your zodiac traits
- **Compatibility Checker**: Check compatibility between two people based on birth dates and personality traits

## Prerequisites

- Node.js (v14.0.0 or higher)
- npm (v6.0.0 or higher)

## Getting Started

Follow these steps to set up the project on your local machine:

### 1. Clone the repository

```bash
git clone <repository-url>
cd zodiacx
```

### 2. Install dependencies

```bash
npm install
```

### 3. Create folder structure

Ensure you have the following folder structure:

```
zodiacx/
├── public/
│   └── images/           # Place zodiac sign images here
│   └── sounds/           # Add hover and click sounds
├── src/
│   ├── assets/           
│   ├── components/       
│   ├── pages/            
│   ├── styles/           
│   ├── App.jsx           
│   ├── main.jsx          
│   └── Router.jsx        
```

### 4. Add images

Place zodiac sign images in the `public/images/` directory with the following naming convention:
- Aries.webp
- Taurus.webp
- Gemini.webp
- Cancer.webp
- Leo.webp
- Virgo.webp
- Libra.webp
- Scorpio.webp
- Sagittarius.webp
- Capricorn.webp
- Aquarius.webp
- Pisces.webp

### 5. Add sounds (optional)

Add the following sound files to the `public/sounds/` directory:
- button-16.mp3 (for hover effect)
- button-30.mp3 (for click effect)

### 6. Start the development server

```bash
npm run dev
```

The application will be available at `http://localhost:3000`

## Building for Production

To create a production build, run:

```bash
npm run build
```

The build artifacts will be stored in the `dist/` directory.

## Project Structure

- `src/components/`: Reusable UI components
- `src/pages/`: Page components for routing
- `src/styles/`: CSS files for styling
- `src/App.jsx`: Main application component
- `src/Router.jsx`: Routing configuration
- `src/main.jsx`: Application entry point

## Technologies Used

- React
- React Router
- Vite
- CSS3 with custom animations

## Credits

This project uses the starry background animation effect and zodiac sign data for educational purposes.

## License

This project is licensed under the MIT License.
