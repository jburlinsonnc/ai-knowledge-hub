# Copilot Instructions

<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

## Project Overview
This is a modern React application built with:
- **React 18** with TypeScript for type safety
- **Vite** for fast development and building
- **Tailwind CSS** for utility-first styling
- **ESLint** for code quality

## Development Guidelines
- Use functional components with React hooks
- Prefer TypeScript for all new files
- Use Tailwind CSS classes for styling instead of custom CSS when possible
- Follow React best practices for component composition
- Use semantic HTML elements for accessibility
- Implement responsive design principles

## Code Style
- Use arrow functions for components
- Use descriptive variable and function names
- Keep components small and focused on a single responsibility
- Use TypeScript interfaces for prop types
- Prefer const assertions and explicit types

## File Structure
- Components should be placed in `src/components/`
- Hooks should be placed in `src/hooks/`
- Utilities should be placed in `src/utils/`
- Types should be placed in `src/types/`
- Assets should be placed in `src/assets/`

## Performance Considerations
- Use React.memo() for expensive components
- Implement proper key props for lists
- Use lazy loading for large components
- Optimize images and assets
