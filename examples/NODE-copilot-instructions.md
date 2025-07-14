# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This is a modern Node.js application built with:
- **Node.js 18+** with TypeScript for type safety
- **Express.js** for web framework
- **ESLint** and **Prettier** for code quality and formatting
- **Jest** for testing
- **Prisma/TypeORM** for database ORM

## Development Guidelines
- Use TypeScript for all new files
- Follow RESTful API design principles
- Use async/await instead of callbacks or .then()
- Implement proper error handling with try/catch blocks
- Use middleware for cross-cutting concerns (auth, logging, validation)
- Follow the MVC or layered architecture pattern
- Use environment variables for configuration

## Code Style
- Use arrow functions for consistency
- Use descriptive variable and function names
- Keep functions small and focused on a single responsibility
- Use TypeScript interfaces for type definitions
- Prefer const over let, avoid var
- Use template literals for string interpolation
- Follow camelCase naming convention

## File Structure
- Controllers should be placed in `src/controllers/`
- Services/Business logic should be placed in `src/services/`
- Models should be placed in `src/models/`
- Middleware should be placed in `src/middleware/`
- Routes should be placed in `src/routes/`
- Utilities should be placed in `src/utils/`
- Types should be placed in `src/types/`
- Database migrations should be placed in `src/migrations/`

## API Design
- Use proper HTTP status codes
- Implement consistent error response format
- Use request validation middleware
- Implement rate limiting for public APIs
- Use proper authentication and authorization
- Document APIs with OpenAPI/Swagger

## Performance Considerations
- Use connection pooling for database connections
- Implement caching where appropriate
- Use compression middleware
- Optimize database queries
- Use streaming for large data transfers
- Implement proper logging without performance impact

## Security Best Practices
- Validate and sanitize all inputs
- Use parameterized queries to prevent SQL injection
- Implement proper authentication and session management
- Use HTTPS in production
- Keep dependencies updated
- Use security headers middleware 