# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This is a modern Python application built with:
- **Python 3.9+** with type hints for better code quality
- **FastAPI/Django/Flask** for web framework
- **SQLAlchemy/Django ORM** for database operations
- **Pydantic** for data validation
- **pytest** for testing
- **Black** and **isort** for code formatting

## Development Guidelines
- Use type hints for all function parameters and return values
- Follow PEP 8 style guidelines
- Use virtual environments for dependency management
- Implement proper error handling with custom exceptions
- Use async/await for I/O operations when possible
- Follow the single responsibility principle
- Use dataclasses or Pydantic models for data structures

## Code Style
- Use snake_case for variables and functions
- Use PascalCase for classes
- Use UPPER_CASE for constants
- Keep line length under 88 characters (Black default)
- Use docstrings for all public functions and classes
- Prefer list comprehensions over loops when readable
- Use f-strings for string formatting

## File Structure
- Views/Routes should be placed in `src/views/` or `src/routes/`
- Business logic should be placed in `src/services/`
- Models should be placed in `src/models/`
- Database schemas should be placed in `src/schemas/`
- Utilities should be placed in `src/utils/`
- Configuration should be placed in `src/config/`
- Tests should be placed in `tests/`
- Requirements should be in `requirements.txt` or `pyproject.toml`

## API Design (FastAPI/Flask)
- Use Pydantic models for request/response validation
- Implement proper HTTP status codes
- Use dependency injection for common operations
- Document APIs with automatic OpenAPI generation
- Implement proper error handling middleware
- Use async endpoints for I/O operations

## Performance Considerations
- Use connection pooling for database connections
- Implement caching with Redis or similar
- Use background tasks for long-running operations
- Optimize database queries with proper indexing
- Use generators for large data processing
- Profile code to identify bottlenecks

## Testing Best Practices
- Write unit tests for all business logic
- Use fixtures for test data setup
- Mock external dependencies
- Aim for high test coverage
- Use parametrized tests for multiple scenarios
- Test both success and failure cases

## Security Best Practices
- Validate all inputs with Pydantic or similar
- Use parameterized queries to prevent SQL injection
- Implement proper authentication and authorization
- Hash passwords with bcrypt or similar
- Use environment variables for secrets
- Keep dependencies updated with security patches 