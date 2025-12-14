# GEMINI.md

## Project Overview

This is a boilerplate React Native project for a Pacman game, built with Expo. The project is in its initial state and contains the default starter code from the Expo template. It uses TypeScript and includes the `react-native-game-engine` library, which suggests that the goal is to build a game.

The project is structured as a standard Expo project with file-based routing. The main screens are located in the `app/(tabs)` directory, and the navigation is set up in `app/_layout.tsx`.

## Building and Running

To get started with this project, follow these steps:

1.  **Install dependencies:**
    ```bash
    npm install
    ```

2.  **Start the app:**
    ```bash
    npx expo start
    ```

    This will open the Expo developer tools in your browser. You can then choose to run the app on an Android emulator, iOS simulator, or on a physical device using the Expo Go app.

### Other available scripts:

*   `npm run android`: Start the app on a connected Android device or emulator.
*   `npm run ios`: Start the app on an iOS simulator.
*   `npm run web`: Start the app in a web browser.
*   `npm run lint`: Lint the code using ESLint.
*   `npm run reset-project`: Reset the project to a blank state, moving the current `app`, `components`, `hooks`, and `constants` directories to an `app-example` directory.

## Development Conventions

The project uses ESLint for code linting, and the configuration is in the `eslint.config.js` file. The project also uses TypeScript, and the configuration is in the `tsconfig.json` file.

Since the project is in its initial state, there are no specific development conventions yet. However, it is recommended to follow the standard React Native and TypeScript best practices.

## Next Steps

To start building the Pacman game, you can begin by creating a new screen for the game and implementing the game logic using the `react-native-game-engine` library. You can create new components for the game in the `components` directory and define the game's theme and constants in the `constants` directory.
