# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This is a modern Next.js application built with:
- **Next.js 13+** with App Router for routing and layouts
- **React 18** with TypeScript for type safety
- **Tailwind CSS** for utility-first styling
- **ESLint** and **Prettier** for code quality and formatting
- **Prisma** or **Drizzle** for database ORM

## Development Guidelines
- Use App Router over Pages Router for new projects
- Implement Server Components by default, Client Components when needed
- Use TypeScript for all new files
- Follow React Server Components best practices
- Use Next.js built-in optimizations (Image, Link, etc.)
- Implement proper SEO with metadata API
- Use streaming and Suspense for better UX

## Code Style
- Use arrow functions for components
- Use descriptive variable and function names
- Keep components small and focused
- Use TypeScript interfaces for prop types
- Prefer const assertions and explicit types
- Use async/await for server-side operations
- Follow Next.js naming conventions

## File Structure (App Router)
- Pages should be placed in `src/app/` with page.tsx files
- Components should be placed in `src/components/`
- Server actions should be placed in `src/app/actions/`
- API routes should be placed in `src/app/api/`
- Utilities should be placed in `src/lib/`
- Types should be placed in `src/types/`
- Database schemas should be placed in `src/db/`
- Middleware should be in `src/middleware.ts`

## Server vs Client Components
- Use Server Components by default for better performance
- Use Client Components only when needed (interactivity, browser APIs)
- Mark Client Components with 'use client' directive
- Keep Client Components small and focused
- Pass data from Server to Client Components as props
- Use Server Actions for form submissions and mutations

## Data Fetching and Caching
- Use fetch with Next.js caching by default
- Implement proper error handling for data fetching
- Use Suspense boundaries for loading states
- Implement proper revalidation strategies
- Use Server Actions for mutations
- Cache API responses appropriately

## Routing and Navigation
- Use App Router file-based routing
- Implement proper layouts and nested layouts
- Use route groups for organization
- Implement proper loading and error pages
- Use parallel routes when appropriate
- Implement proper middleware for authentication

## SEO and Metadata
- Use the Metadata API for SEO optimization
- Implement proper Open Graph and Twitter cards
- Use structured data when appropriate
- Implement proper canonical URLs
- Use Next.js Image component for optimization
- Implement proper sitemap generation

## Performance Optimization
- Use Next.js Image component for image optimization
- Implement proper code splitting with dynamic imports
- Use Suspense for better loading experiences
- Optimize fonts with next/font
- Use proper caching strategies
- Implement proper bundle analysis

## API Routes and Server Actions
- Use route handlers for API endpoints
- Implement proper error handling in API routes
- Use middleware for authentication and validation
- Implement proper CORS policies
- Use Server Actions for form handling
- Implement proper request validation

## Database and ORM
- Use Prisma or Drizzle for database operations
- Implement proper database migrations
- Use connection pooling for better performance
- Implement proper error handling for database operations
- Use transactions for complex operations
- Implement proper data validation

## Authentication and Security
- Use NextAuth.js or similar for authentication
- Implement proper session management
- Use middleware for route protection
- Implement proper CSRF protection
- Validate all inputs on server side
- Use environment variables for secrets

## Testing Best Practices
- Write unit tests for utilities and components
- Use Jest and React Testing Library
- Test Server Components and Client Components separately
- Mock external dependencies
- Test API routes with proper mocking
- Implement e2e tests for critical paths

## Deployment and Production
- Use Vercel or similar platforms for deployment
- Implement proper environment variable management
- Use proper build optimization
- Implement proper monitoring and logging
- Use CDN for static assets
- Implement proper error tracking 