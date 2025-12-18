# Build, Test, and Lint Commands

This document outlines the available commands for building, testing, and linting the application, based on the scripts defined in `package.json` and repository configuration.

## Build Commands

### Development Server

- **Command**: `npm run dev` or `yarn dev`
- **Description**: Starts the Vite development server for local development.
- **Expected Outcome**: Launches a local server (typically on `http://localhost:5173`) with hot module replacement enabled.
- **Common Flags**: None specified in scripts.
- **Troubleshooting**: Ensure port 5173 is available. If conflicts occur, Vite may automatically suggest an alternative port.

### Production Build

- **Command**: `npm run build` or `yarn build`
- **Description**: Creates an optimized production build using Vite.
- **Expected Outcome**: Generates a `dist/` folder with minified and bundled assets ready for deployment.
- **Common Flags**: None specified in scripts.
- **Troubleshooting**: Check for any build errors in the console output. Ensure all dependencies are installed.

### Preview Production Build

- **Command**: `npm run preview` or `yarn preview`
- **Description**: Serves the production build locally for testing before deployment.
- **Expected Outcome**: Starts a local server to preview the built application.
- **Common Flags**: None specified in scripts.
- **Troubleshooting**: Requires a successful build first. Run `npm run build` before previewing.

## Lint Commands

### ESLint

- **Command**: `npm run lint` or `yarn lint`
- **Description**: Runs ESLint on the entire project to check for code quality issues and style violations.
- **Expected Outcome**: Reports any linting errors or warnings in the console. Exit code 0 if no issues, 1 if issues found.
- **Common Flags**: None specified in scripts. ESLint uses the configuration in `eslint.config.js`.
- **Troubleshooting**:
  - Install dependencies if ESLint is not found.
  - Check `eslint.config.js` for configuration issues.
  - Use `--fix` flag manually if available to auto-fix some issues: `npx eslint . --fix`

## Test Commands

- **No test commands are configured** in this repository.
- There are no test scripts in `package.json`.
- No testing framework (Jest, Vitest, etc.) is installed.
- No CI/CD configuration files (GitHub Actions, etc.) are present for automated testing.

## CI/CD Configuration

- No CI/CD pipelines are configured in this repository.
- No workflow files in `.github/workflows/` or similar CI configuration files detected.
