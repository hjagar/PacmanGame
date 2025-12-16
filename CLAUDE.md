# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a React Native Pacman game project built with Expo and TypeScript. The project uses `react-native-game-engine` (v1.2.0) for game development. Currently in early development stage with minimal implementation - the app structure has been cleaned from the default Expo template.

## Tech Stack

- **Framework**: Expo SDK ~54.0.27 with React Native 0.81.5 and React 19.1.0
- **Routing**: Expo Router 6.0.17 (file-based routing)
- **Language**: TypeScript 5.9.2 with strict mode enabled
- **Game Engine**: react-native-game-engine 1.2.0
- **Navigation**: React Navigation v7 with bottom tabs support
- **Linting**: ESLint 9.25.0 with expo config

## Development Commands

### Starting the app
```bash
npm start              # Start Expo dev server
npm run android        # Run on Android device/emulator
npm run ios            # Run on iOS simulator
npm run web            # Run in web browser
```

### Code quality
```bash
npm run lint           # Run ESLint
```

### Resetting project
```bash
npm run reset-project  # Moves app/, components/, hooks/, constants/ to app-example/
```

## Project Structure

- **app/**: Main application code using Expo Router file-based routing
  - `app/_layout.tsx`: Root layout with Stack navigator
  - `app/index.tsx`: Entry screen (currently a placeholder)
- **components/**: Reusable UI components (currently empty after cleanup)
- **constants/**: App-wide constants (currently empty after cleanup)
- **hooks/**: Custom React hooks (currently empty after cleanup)

## Path Aliases

The project uses `@/*` path alias for imports, configured in tsconfig.json:
```typescript
import { Component } from '@/components/Component';
```

## Architecture Notes

### Expo Router File-Based Routing
This project uses Expo Router for navigation. File structure in the `app/` directory determines routes:
- `app/index.tsx` → `/` route
- `app/_layout.tsx` → Defines layout wrapper and navigation structure
- Future screens should be added as files/folders in `app/`

### Game Engine Integration
The project includes `react-native-game-engine` which provides:
- A game loop for rendering and updates
- Entity-component system for game objects
- Touch handling for game interactions

When implementing game features, use the GameEngine component from `react-native-game-engine` and structure game logic around entities and systems.

## Current State

The project is in initial development. Most boilerplate code from the Expo template has been removed (as seen in git status). The next steps involve implementing the Pacman game logic, entities (Pacman, ghosts, pellets, maze), and game systems (collision detection, movement, scoring).
