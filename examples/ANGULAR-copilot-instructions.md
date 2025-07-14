# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This is a modern Angular application built with:
- **Angular 15+** with TypeScript for type safety
- **Angular CLI** for project scaffolding and build tools
- **RxJS** for reactive programming
- **Angular Material** or **PrimeNG** for UI components
- **ESLint** and **Prettier** for code quality and formatting

## Development Guidelines
- Use Angular CLI for generating components, services, and modules
- Follow reactive programming patterns with RxJS
- Use TypeScript strict mode for better type safety
- Implement proper component lifecycle management
- Use Angular's dependency injection system
- Follow the single responsibility principle
- Use OnPush change detection strategy when appropriate

## Code Style
- Use PascalCase for classes and interfaces
- Use camelCase for methods and properties
- Use kebab-case for selectors and file names
- Use UPPER_CASE for constants
- Use descriptive names for components and services
- Follow Angular naming conventions
- Use readonly for properties that shouldn't change

## File Structure
- Components should be placed in `src/app/components/`
- Services should be placed in `src/app/services/`
- Models/Interfaces should be placed in `src/app/models/`
- Guards should be placed in `src/app/guards/`
- Interceptors should be placed in `src/app/interceptors/`
- Pipes should be placed in `src/app/pipes/`
- Modules should be placed in `src/app/modules/`
- Shared utilities should be placed in `src/app/shared/`

## Component Best Practices
- Use OnPush change detection strategy for better performance
- Implement OnDestroy to prevent memory leaks
- Use trackBy functions for *ngFor loops
- Keep templates simple and move logic to component classes
- Use async pipe for observables in templates
- Implement proper error handling
- Use ViewChild and ContentChild appropriately

## Service and Dependency Injection
- Use providedIn: 'root' for singleton services
- Implement proper error handling in services
- Use HTTP interceptors for cross-cutting concerns
- Return observables from service methods
- Use dependency injection for testing
- Implement proper service lifecycle management

## Reactive Programming with RxJS
- Use observables for asynchronous operations
- Implement proper error handling with catchError
- Use operators like map, filter, switchMap appropriately
- Unsubscribe from observables to prevent memory leaks
- Use subjects for component communication
- Implement proper stream composition

## Forms and Validation
- Use reactive forms over template-driven forms
- Implement custom validators when needed
- Use form builders for complex forms
- Implement proper form validation feedback
- Use form arrays for dynamic forms
- Handle form submission and errors properly

## Routing and Navigation
- Use lazy loading for feature modules
- Implement route guards for authentication and authorization
- Use resolvers for data fetching before navigation
- Implement proper error handling for routes
- Use route parameters and query parameters appropriately
- Implement breadcrumb navigation when needed

## Testing Best Practices
- Write unit tests for components and services
- Use TestBed for component testing
- Mock dependencies in tests
- Use async and fakeAsync for asynchronous testing
- Test component interactions and outputs
- Use Page Object Model for e2e tests

## Performance Optimization
- Use OnPush change detection strategy
- Implement lazy loading for modules
- Use trackBy functions for lists
- Optimize bundle size with tree shaking
- Use Angular Universal for server-side rendering
- Implement proper caching strategies
- Use web workers for heavy computations

## Security Best Practices
- Sanitize user inputs to prevent XSS
- Use Angular's built-in security features
- Implement proper authentication and authorization
- Use HTTPS in production
- Validate data on both client and server
- Use Content Security Policy headers 