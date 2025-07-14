# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This project uses containerization best practices including:
- **Docker** for application containerization
- **Docker Compose** for local development environments
- **Multi-stage builds** for optimized production images
- **Container security** scanning and best practices
- **Kubernetes** deployment configurations

## Development Guidelines
- Use official base images when possible
- Implement multi-stage builds for smaller production images
- Use specific image tags, avoid 'latest' in production
- Run containers as non-root users
- Use .dockerignore to exclude unnecessary files
- Keep images minimal and focused
- Use health checks for container monitoring

## Dockerfile Best Practices
- Use multi-stage builds to reduce image size
- Order layers from least to most frequently changing
- Use COPY instead of ADD unless specific functionality needed
- Combine RUN commands to reduce layers
- Use specific versions for base images
- Clean up package caches in the same RUN command
- Use WORKDIR instead of cd commands

## Container Security
- Run containers as non-root users
- Use minimal base images (Alpine, distroless)
- Scan images for vulnerabilities regularly
- Use secrets management for sensitive data
- Implement proper network policies
- Use read-only filesystems when possible
- Limit container resources (CPU, memory)

## Docker Compose Guidelines
- Use environment-specific compose files
- Use external networks for service communication
- Implement proper service dependencies
- Use volumes for persistent data
- Configure proper restart policies
- Use healthchecks for service monitoring
- Implement proper logging configuration

## File Structure
- Dockerfiles should be in project root or `docker/`
- Docker Compose files should be in project root
- Docker-related scripts should be in `scripts/docker/`
- Container configurations should be in `docker/configs/`
- Build contexts should be optimized with .dockerignore

## Image Optimization
- Use multi-stage builds to separate build and runtime dependencies
- Minimize the number of layers
- Use .dockerignore to exclude unnecessary files
- Choose appropriate base images for your use case
- Clean up temporary files in the same RUN command
- Use specific package versions for reproducible builds

## Environment Management
- Use environment variables for configuration
- Use .env files for local development
- Implement different configurations for different environments
- Use Docker secrets for sensitive data in production
- Validate environment variables at startup
- Document all required environment variables

## Networking and Communication
- Use custom networks for service isolation
- Implement proper service discovery
- Use environment variables for service endpoints
- Configure proper port mappings
- Implement load balancing for scalable services
- Use reverse proxies for external access

## Data Management
- Use named volumes for persistent data
- Implement proper backup strategies for volumes
- Use bind mounts for development only
- Configure proper volume permissions
- Implement data migration strategies
- Use init containers for data setup

## Monitoring and Logging
- Implement proper logging strategies
- Use structured logging formats
- Configure log rotation and retention
- Implement health checks for all services
- Use monitoring tools for container metrics
- Set up alerting for container failures

## CI/CD Integration
- Build images in CI/CD pipelines
- Use multi-stage builds for different environments
- Implement proper tagging strategies
- Scan images for vulnerabilities in CI/CD
- Use registry caching for faster builds
- Implement proper deployment strategies

## Performance Considerations
- Use appropriate resource limits and requests
- Implement proper caching strategies
- Use init systems for proper signal handling
- Optimize startup time
- Use appropriate JVM settings for Java applications
- Implement proper graceful shutdown procedures 