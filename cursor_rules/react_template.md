# NOTES: Make sure to update the project context and tech stack to match the project you are working on.

# [Project Name]

Every time you choose to apply a rule(s), explicitly state the rule(s) in the output. You can abbreviate the rule description to a single word or phrase.

## Project Context

[Brief description]

-   [more description]
-   [more description]
-   [more description]

## Code Style and Structure

-   Write concise, technical TypeScript code with accurate examples
-   Use functional and declarative programming patterns; avoid classes
-   Prefer iteration and modularization over code duplication
-   Use descriptive variable names with auxiliary verbs (e.g., isLoading, hasError)
-   After every change make sure to refine the code and remove any unused code
-   After every change ask if I want to commit the changes, if not, just continue
-   Structure repository files as follows:

```plaintext
structure of the project
```

## Tech Stack and Dependencies

-   **Frontend**: React, Vite, TypeScript, Tailwind CSS, Shadcn UI
-   **Backend**: Express.js, Prisma, PostgreSQL
-   **State Management**: TanStack Query, Zustand
-   **Utilities**: React Router, React Hook Form, Zod

## Naming Conventions

-   Use lowercase with dashes for directories (e.g., components/form-wizard)
-   Favor named exports for components and utilities
-   Use PascalCase for component files (e.g., VisaForm.tsx)
-   Use camelCase for utility files (e.g., formValidator.ts)

## TypeScript Usage

-   Use TypeScript for all code; prefer interfaces over types
-   Avoid enums; use const objects with 'as const' assertion
-   Use functional components with TypeScript interfaces
-   Use absolute imports with aliasing for all files @/...
-   Avoid try/catch blocks unless there's good reason to translate or handle error in that abstraction
-   Use explicit return types for all functions

## State Management

-   Use React Context for its intended purpose of avoiding extreme prop drilling
-   Use TanStack Query for data fetching
-   Use Zustand for state management
-   Implement proper cleanup in useEffect hooks
-   Avoid running extra API calls such as unnecessary GET requests. Use TanStack Query’s cache and responses from POST/PUT calls, or implement optimistic updates to manage state changes efficiently.

## Syntax and Formatting

-   Use "function" keyword for pure functions
-   Avoid unnecessary curly braces in conditionals
-   Use declarative JSX
-   For TanStack Query, follow common practices such as 1 hook per file and organize multiple hooks into a separate folder
-   Keep components small and focused
-   Implement Lazy Loading for components and routes when applicable

## UI and Styling

-   Use Shadcn UI and Radix for components
-   Use `npx shadcn@latest add <component-name>` to add new shadcn components
-   Implement Tailwind CSS for styling
-   When adding new Shadcn component, document the installation command
-   Make sure the app is responsive on desktop, tablet, and mobile

## Error Handling

-   Implement proper error boundaries
-   Log errors appropriately for debugging
-   Provide user-friendly error messages
-   Handle network failures gracefully

## Performance Optimization

-   Use memoization (e.g., `React.memo`, `useMemo`, `useCallback`) to avoid unnecessary renders.
-   Optimize large lists with virtualized rendering.

## Testing

-   Write unit tests for utilities and components
-   Implement E2E tests for critical flows
-   Test across different Chrome versions
-   Test memory usage and performance

## Security

-   Sanitize user inputs
-   Handle sensitive data properly

## Git Usage

Commit Message Prefixes:

-   "fix:" for bug fixes
-   "feat:" for new features
-   "perf:" for performance improvements
-   "docs:" for documentation changes
-   "style:" for formatting changes
-   "refactor:" for code refactoring
-   "test:" for adding missing tests
-   "chore:" for maintenance tasks

Rules:

-   Use lowercase for commit messages
-   Keep the summary line concise
-   Include description for non-obvious changes
-   Reference issue numbers when applicable

## Documentation

-   Maintain clear README with setup instructions
-   Update the README, .cursorrules, and .env files immediately after significant changes as needed
-   Document API interactions and data flows
-   Include comments for algorithms or processes that aren't intuitive
-   Don't include comments unless it's for complex logic
-   Update documentation immediately after significant changes
-   Don't remove existing comments without a good reason

## Development Workflow

-   Use proper version control
-   Implement proper code review process
-   Follow semantic versioning for releases
-   Maintain changelog
