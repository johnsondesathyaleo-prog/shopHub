# Coding Standards

This document outlines the coding standards and conventions observed in this React-based e-commerce application repository. These standards are derived from the actual patterns used in the codebase.

## Naming Conventions

### Components and Files

- **React Components**: PascalCase for component names and filenames (e.g., `Button.jsx`, `Header.jsx`, `ProductCard.jsx`).
- **Hooks**: camelCase prefixed with `use` (e.g., `useForm.js`, `useCarousel.js`).
- **Contexts**: PascalCase with `Context` suffix (e.g., `AuthContext.jsx`, `CartContext.jsx`).
- **Pages**: PascalCase with `Page` suffix (e.g., `LoginPage.jsx`, `CartPage.jsx`).
- **Utilities**: camelCase (e.g., `formatters.js`, `validators.js`).
- **Constants**: UPPER_CASE with descriptive names (e.g., `routes.js` containing `ROUTES` object).

### Variables and Functions

- **Variables**: camelCase (e.g., `user`, `isAuthenticated`, `initialValues`).
- **Functions**: camelCase (e.g., `login`, `handleChange`, `handleBlur`).
- **Constants**: UPPER_CASE for object keys in constants files (e.g., `HOME`, `LOGIN` in `ROUTES`).

### CSS Classes

- **Base Classes**: kebab-case (e.g., `btn`, `main-content`).
- **Modifier Classes**: kebab-case with prefixes (e.g., `btn-primary`, `btn-full-width`).

## Formatting Rules

### JavaScript/JSX

- Use 2 spaces for indentation.
- Single quotes for string literals.
- Semicolons are used.
- Object and array literals use consistent formatting with proper indentation.
- Destructuring is preferred for props and state variables.
- Template literals are used for dynamic class names and strings.

### CSS

- Standard CSS formatting with 2 spaces indentation.
- Properties in logical order (e.g., sizing, colors, effects).
- Use of `rem` units for scalable sizing.
- Vendor prefixes not observed (modern browser targeting assumed).

## Component and Folder Structure

### Component Organization

- Each component resides in its own folder containing `.jsx` and `.css` files.
- Components are organized into subfolders: `common/` for shared components, `features/` for feature-specific components, `layout/` for layout components.
- Default exports are used for components.

### Folder Hierarchy

- `src/components/`: All reusable components.
- `src/pages/`: Page-level components corresponding to routes.
- `src/context/`: React Context providers.
- `src/hooks/`: Custom React hooks.
- `src/utils/`: Utility functions.
- `src/constants/`: Application constants and data.

## State Management Patterns

### React Context

- State is managed using React Context API with provider components (`AuthProvider`, `CartProvider`).
- Custom hooks are provided for consuming context (`useAuth`).
- Context consumers throw errors if used outside providers.
- State updates are handled through functions exposed in the context value.

### Local State

- `useState` hook is used for component-level state.
- State variables follow camelCase naming.
- Multiple related state variables are grouped logically.

## Typing Conventions

- No TypeScript files are used in the codebase.
- TypeScript definition files (`@types/react`, `@types/react-dom`) are included in devDependencies for development-time type checking.
- Prop types are not explicitly validated (no PropTypes or similar libraries).

## CSS Standards and Methodology

### CSS Organization

- Each component has its own CSS file imported directly.
- CSS Modules are not used; global class names are employed.
- BEM-like methodology is followed with base classes and modifiers (e.g., `btn btn-primary`).

### Styling Patterns

- CSS custom properties (variables) are not observed.
- Gradients and transitions are used for visual effects.
- Responsive design patterns are not explicitly implemented in the provided CSS.
- Font-family inheritance is used (`font-family: inherit`).

## Testing Conventions

- No testing framework or conventions are implemented in this repository.
- There are no test files, test scripts, or testing-related dependencies.
- Unit tests, integration tests, or end-to-end tests are not present.
