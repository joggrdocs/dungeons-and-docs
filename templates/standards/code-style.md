<!--  
�� Usage:  
- Replace all {{placeholders}} with your organization's content
- Update links and remove unnecessary sections
- Customize as needed 

Happy documenting! 🚀  
-->

# 👨‍💻 Code Style Standards

This document outlines the code style standards for {{ team-name }} to ensure consistent, readable, and maintainable code across our organization.

## 🎯 Core Principle

> You cannot tell who wrote the code, only that someone on the {{ team-name }} did.

## 📝 Naming Conventions

### Variables & Functions

Use `camelCase` for variables and functions:

```typescript
const userName = 'JohnDoe';
function getUserData() {
  // function logic
}
```

### Classes & Components

Use `PascalCase` for classes and components:

```typescript
class UserProfile {
  constructor(name) {
    this.name = name;
  }
}

function App() {
  return <UserProfile name="John" />;
}
```

### Constants

Use `UPPER_CASE` for constants:

```typescript
const API_KEY = '12345-ABCDE';
const MAX_USERS = 100;
```

### File Names

Use `kebab-case` for file names:

```typescript
user-profile.js
dashboard-view.tsx
```

## 💬 Comments & Documentation

### Function Documentation

Use JSDoc for documenting functions and APIs:

```typescript
/**
 * Retrieves user data from the API
 * @param {string} userId - The unique identifier of the user
 * @returns {Promise<UserData>} The user's data
 * @throws {Error} If the user is not found
 */
async function getUserData(userId) {
  // implementation
}
```

### File Organization

- Use header comments for large files only
- Use section comments for organizing large logic blocks
- Avoid redundant comments – describe intent, not obvious functionality

## 🛠️ Linting & Formatting

### Tools

- **Linting**: {{ linting-tool }}
- **Formatting**: {{ formatting-tool }}
- **Type Checking**: {{ type-checking-tool }}

### Configuration

#### Prettier Config

```json
{
  "printWidth": 80,
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true,
  "trailingComma": "es5",
  "arrowParens": "always"
}
```

#### Prettier Ignore

```plaintext
# Basics
dist/
node_modules/
build/
# Docs
*.md
*.mdx
# DevTools
.yarn
.turbo
.vscode
# Fixtures
**/__fixtures__/
**/fixtures/
```

## 🔍 Code Review Standards

### Linting Requirements

- No linting errors in PRs
- All new code must pass type checking
- Follow existing patterns in the codebase

### Documentation Requirements

- Update relevant documentation
- Add JSDoc comments for new functions
- Update README if needed

## 📚 Additional Resources

- [{{ team-name }} Engineering Handbook](../handbook.md)
- [Architecture Standards](./architecture.md)
- [Testing Standards](./testing.md)
- [Git Workflow](./git-workflow.md)
