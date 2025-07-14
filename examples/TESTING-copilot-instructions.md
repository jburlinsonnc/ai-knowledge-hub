# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This project follows comprehensive testing practices including:
- **Unit Testing** with Jest/pytest/JUnit
- **Integration Testing** for API endpoints and database operations
- **End-to-End Testing** with Cypress/Playwright/Selenium
- **Test-Driven Development (TDD)** where appropriate
- **Code Coverage** monitoring and reporting

## Development Guidelines
- Write tests before or alongside production code
- Follow the AAA pattern (Arrange, Act, Assert)
- Use descriptive test names that explain the scenario
- Keep tests independent and isolated
- Mock external dependencies appropriately
- Aim for high test coverage (80%+ for critical paths)
- Use different test types for different purposes

## Test Structure and Naming
- Use descriptive test names: `should_return_user_when_valid_id_provided`
- Group related tests in test suites or describe blocks
- Use setup and teardown methods for common test data
- Keep test files close to the code they test
- Use consistent naming conventions across the project

## Unit Testing Best Practices
- Test one thing at a time
- Use mocks and stubs for external dependencies
- Test both happy path and edge cases
- Test error conditions and exception handling
- Keep tests fast and independent
- Use parameterized tests for multiple scenarios
- Assert on behavior, not implementation details

## Integration Testing Guidelines
- Test API endpoints with real HTTP requests
- Test database operations with test databases
- Test service integrations with contract testing
- Use test containers for external dependencies
- Test authentication and authorization flows
- Verify error handling across service boundaries

## End-to-End Testing Standards
- Test critical user journeys
- Use page object model for UI tests
- Keep E2E tests stable and reliable
- Run E2E tests in CI/CD pipeline
- Use data-testid attributes for element selection
- Test across different browsers and devices

## File Structure
- Unit tests should be placed alongside source files or in `tests/unit/`
- Integration tests should be placed in `tests/integration/`
- E2E tests should be placed in `tests/e2e/`
- Test utilities should be placed in `tests/utils/`
- Test fixtures should be placed in `tests/fixtures/`
- Test configuration should be in `tests/config/`

## Test Data Management
- Use factories or builders for test data creation
- Use fixtures for reusable test data
- Clean up test data after each test
- Use realistic but anonymized data
- Avoid hardcoded values in tests
- Use constants for test data values

## Mocking and Stubbing
- Mock external APIs and services
- Stub time-dependent functions
- Use dependency injection for easier testing
- Mock at the boundary of your system
- Verify mock interactions when necessary
- Reset mocks between tests

## Performance Testing
- Test API response times
- Test database query performance
- Test memory usage and leaks
- Test concurrent user scenarios
- Use profiling tools to identify bottlenecks
- Set performance benchmarks and alerts

## Security Testing
- Test authentication and authorization
- Test input validation and sanitization
- Test for common vulnerabilities (OWASP Top 10)
- Test rate limiting and throttling
- Test data encryption and decryption
- Test session management and timeouts 