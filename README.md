# React Theme Toggle App

This is a React application that allows users to toggle between light and dark themes. The theme mode is applied globally across the app, and the selected theme persists during navigation.

## Features:
- **Light and Dark Theme Toggle**: Users can toggle between light and dark modes using a custom switch.
- **Dynamic Styling**: The theme is applied dynamically, changing the appearance of the app in real-time.
- **Context API**: The `ThemeContext` is used to manage the global theme state and pass the current theme to all components.

## Tech Stack:
- **React** (Frontend)
- **TailwindCSS** (Styling)
- **Context API** (State Management)
- **JavaScript (ES6+)**

## Installation & Setup:

To run this app locally, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/your-username/react-theme-toggle-app.git
   cd react-theme-toggle-app


2. Install Dependencies:

    Make sure you have Node.js installed. If not, download and install it from nodejs.org.

    Then, install the project dependencies using npm or yarn:

    ```bash
    npm install
    # or
    yarn install
    ```

3. Start the Development Server:

    After installing the dependencies, start the development server:

    ```bash
    npm start
    # or
    yarn star 
    ```

    This will open the app in your default browser at http://localhost:5173.

4. File Structure:
    ```graphql
    src/
    │
    ├── components/
    │   ├── Card.js          # Displays the product     card
    │   └── ThemeBtn.js      # The theme toggle button  component
    │
    ├── Context/
    │   └── Theme.js         # Contains the ThemeContext and hooks for managing the theme
    │
    ├── App.js               # Main app component
    └── App.css              # TailwindCSS styles

    ```

## How It Works:

### Theme Context:
- The ThemeContext is created using React's Context API. It provides the current theme (themeMode), as well as functions to toggle between light and dark modes (darkTheme and lightTheme).
- The useTheme hook is used to access the theme state in any component that needs it.

### Theme Toggle:
- The ThemeBtn component renders a toggle switch. When clicked, it changes the theme by calling the darkTheme or lightTheme functions from the useTheme hook.
- The useEffect hook in App.js ensures that the global theme (on the <html> element) updates when the themeMode state changes.

### Responsive Design:
- TailwindCSS is used to style the app, making it responsive and easy to maintain. The app layout adjusts seamlessly to different screen sizes.


## Demo:
This app dynamically changes its theme when toggling the switch. Check out the live demo:

[Live Demo Link](https://github.com)

## Contributing:
If you'd like to contribute to this project, feel free to fork the repository and submit a pull request.
