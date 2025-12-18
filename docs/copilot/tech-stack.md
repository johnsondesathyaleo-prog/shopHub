# Tech Stack Analysis

## High-Level Purpose

This repository contains a React-based e-commerce application that provides users with the ability to browse products, manage a shopping cart, proceed through checkout, and handle user authentication. The application is structured as a single-page application (SPA) with multiple pages for different functionalities.

## UI Frameworks and Libraries

- **React**: Version 19.2.0 - Primary UI framework for building the user interface components.
- **React Router DOM**: Version 7.9.6 - Used for client-side routing between different pages (e.g., product listing, cart, checkout).

## Languages Used

- **JavaScript**: Primary language for all source files (.jsx, .js).
- **TypeScript Definitions**: Included via @types/react and @types/react-dom for type checking support in development.

## Styling Approach

- **CSS**: Standard CSS files used for styling components and pages. Each component has its own .css file (e.g., Button.css, App.css).
- **CSS Modules**: Not explicitly used; styles are imported directly in components.

## Build Tools

- **Vite**: Version 7.2.4 - Modern build tool for development server, bundling, and production builds. Uses @vitejs/plugin-react for React support.

## Linting Tools

- **ESLint**: Version 9.39.1 - Configured with React-specific plugins (eslint-plugin-react-hooks, eslint-plugin-react-refresh) for code quality and error detection.

## Testing Tools

- No testing tools or frameworks are configured in this repository. There are no test scripts in package.json or testing-related dependencies.

## Folder Structure Patterns

The project follows a modular folder structure under `src/`:

- `components/`: Reusable UI components organized into `common/` (shared components like Button, Input), `features/` (feature-specific like ProductCard), and `layout/` (layout components like Header).
- `pages/`: Page-level components for different routes (e.g., ProductListingPage, CartPage).
- `context/`: React Context providers for state management (AuthContext, CartContext).
- `hooks/`: Custom React hooks (useCarousel, useForm).
- `utils/`: Utility functions (formatters, validators).
- `constants/`: Application constants (enums, productData, routes).
- `assets/`: Static assets (not detailed in structure).
