# Copilot Instructions

This repository contains a React-based e-commerce application for browsing products, managing carts, and processing orders.

## Documentation References

- See [docs/copilot/tech-stack.md](docs/copilot/tech-stack.md) for technology stack and project structure details.
- See [docs/copilot/coding-standards.md](docs/copilot/coding-standards.md) for coding conventions and patterns.
- See [docs/copilot/build-test.md](docs/copilot/build-test.md) for build, lint, and development commands.

## Behavioral Guidelines

- Follow the established naming conventions and component structure patterns when creating new code.
- Use React Context for state management as demonstrated in existing contexts.
- Maintain separate CSS files for each component with BEM-like class naming.
- Run `npm run lint` to ensure code quality before committing changes.
- Use `npm run dev` for development and `npm run build` for production builds.
- Prefer functional components with hooks over class components.
- Import styles directly in component files as shown in existing code.
- Use camelCase for variables and functions, PascalCase for components.
- Avoid adding testing frameworks or CI/CD without explicit requirements.
