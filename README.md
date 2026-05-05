# Theme Switcher

A React + Vite application demonstrating light/dark theme switching using React Context API and Tailwind CSS.

## Features

- **Light/Dark Theme Toggle** - Toggle switch to change between light and dark themes
- **Product Card Display** - Sample Apple Watch product card with image, rating stars, price, and "Add to cart" button
- **Context API** - Uses React Context for global theme state management
- **Tailwind CSS** - Responsive styling with built-in dark mode support

## Tech Stack

- React 18
- Vite
- Tailwind CSS
- React Context API
- ESLint

## Project Structure

```
src/
├── components/
│   ├── Card.jsx        # Product card component
│   └── ThemeBtn.jsx   # Theme toggle button
├── contexts/
│   └── theme.js       # Theme Context (createContext, useContext)
├── App.jsx            # Main app with theme provider
├── main.jsx           # Entry point
└── index.css          # Global styles
```

## Setup

1. Install dependencies:
```bash
npm install
```

2. Start development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

## How It Works

- **ThemeBtn** component provides a checkbox toggle that calls `darkTheme()` or `lightTheme()` functions
- **App.jsx** manages theme state with `useState` and applies theme class to `<html>` element via `useEffect`
- **ThemeContext** provides theme values globally using React Context API
- **Card** component displays differently based on current theme (light/dark classes)

## Default Theme

The app starts in **light** mode by default. Click the toggle switch to switch to dark mode.
