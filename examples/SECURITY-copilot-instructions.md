# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This project follows comprehensive security practices including:
- **OWASP Top 10** vulnerability prevention
- **Zero Trust Architecture** principles
- **Secure by Design** development approach
- **Regular Security Audits** and penetration testing
- **Compliance** with industry standards (SOC 2, GDPR, etc.)

## Development Guidelines
- Follow the principle of least privilege
- Validate and sanitize all inputs
- Use secure coding practices from the start
- Implement defense in depth
- Never trust user input or external data
- Use established security libraries and frameworks
- Keep security patches up to date

## Authentication and Authorization
- Use strong password policies and multi-factor authentication
- Implement proper session management
- Use JWT tokens with appropriate expiration
- Implement role-based access control (RBAC)
- Use OAuth 2.0 or OpenID Connect for third-party authentication
- Never store passwords in plain text
- Use secure password hashing (bcrypt, scrypt, Argon2)

## Input Validation and Sanitization
- Validate all inputs on both client and server side
- Use parameterized queries to prevent SQL injection
- Sanitize data before displaying to prevent XSS
- Implement proper file upload validation
- Use Content Security Policy (CSP) headers
- Validate file types and sizes for uploads
- Use allowlists instead of blocklists when possible

## Data Protection
- Encrypt sensitive data at rest and in transit
- Use HTTPS/TLS for all communications
- Implement proper key management
- Use environment variables for secrets
- Never commit secrets to version control
- Implement data masking for logs and debugging
- Follow data retention and deletion policies

## API Security
- Use API keys or tokens for authentication
- Implement rate limiting and throttling
- Use proper HTTP status codes
- Implement CORS policies appropriately
- Use API versioning for backward compatibility
- Log and monitor API usage
- Implement request/response validation

## Error Handling and Logging
- Don't expose sensitive information in error messages
- Log security events and failed authentication attempts
- Use structured logging for security monitoring
- Implement proper error handling without information leakage
- Monitor for suspicious activities and patterns
- Use centralized logging for security analysis

## File Structure
- Security configurations should be placed in `src/security/`
- Authentication middleware should be placed in `src/middleware/auth/`
- Security utilities should be placed in `src/utils/security/`
- Security tests should be placed in `tests/security/`
- Security documentation should be in `docs/security/`

## Dependency Management
- Regularly update dependencies to patch vulnerabilities
- Use dependency scanning tools
- Review third-party libraries for security issues
- Use package lock files to ensure consistent versions
- Monitor for security advisories
- Use tools like npm audit, pip-audit, or similar

## Infrastructure Security
- Use secure container images and scan for vulnerabilities
- Implement network segmentation and firewalls
- Use secrets management systems (HashiCorp Vault, AWS Secrets Manager)
- Enable security monitoring and alerting
- Use infrastructure as code for consistent security configurations
- Implement backup and disaster recovery procedures

## Code Review Security Checklist
- Review for common vulnerabilities (OWASP Top 10)
- Check for hardcoded secrets or credentials
- Verify proper input validation and sanitization
- Review authentication and authorization logic
- Check for secure communication protocols
- Verify error handling doesn't leak information
- Review logging for security events

## Compliance and Auditing
- Maintain audit trails for security-relevant actions
- Implement data privacy controls (GDPR, CCPA)
- Document security procedures and policies
- Conduct regular security assessments
- Implement change management processes
- Maintain incident response procedures 