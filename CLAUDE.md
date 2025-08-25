# Claude Code Configuration

## Code Standards

### General Guidelines
- Use consistent indentation (2 spaces for JS/TS/JSON, 4 spaces for Python)
- Follow semantic naming conventions
- Write self-documenting code
- Use TypeScript for type safety when applicable
- Follow modern ES6+ syntax

### Code Style
- Use camelCase for variables and functions
- Use PascalCase for classes and components
- Use UPPER_SNAKE_CASE for constants
- Prefer const over let, avoid var
- Use template literals for string interpolation
- Use arrow functions for callbacks and short functions

### Project Structure
```
src/
  components/
  pages/
  utils/
  types/
  styles/
tests/
docs/
```

## Settings Configuration

### VS Code Settings (settings.json)
```json
{
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "editor.detectIndentation": false,
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.organizeImports": true
  },
  "typescript.preferences.importModuleSpecifier": "relative",
  "javascript.preferences.importModuleSpecifier": "relative",
  "files.exclude": {
    "node_modules": true,
    "dist": true,
    "build": true
  }
}
```

### ESLint Configuration
- Use Prettier for code formatting
- Enable TypeScript ESLint rules
- Configure import/export rules
- Set up React hooks rules if using React

### Git Configuration
- Use conventional commits
- Set up pre-commit hooks for linting
- Configure .gitignore for node_modules, dist, .env files

## Development Commands

### Common Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run test` - Run tests
- `npm run lint` - Run linter
- `npm run type-check` - Run TypeScript type checking

### Testing
- Use Jest for unit tests
- Use React Testing Library for component tests
- Maintain minimum 80% test coverage
- Write integration tests for critical paths