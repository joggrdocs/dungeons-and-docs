# 📐 Repository Code Style Guide Template

This document provides a template for code style guides in Spellforge Technologies repositories.

## ✨ Example CODE_STYLE.md

```markdown
# 📐 Arcane API Code Style Guide

This guide outlines the coding standards and conventions for the Arcane API repository.

## 🧙‍♂️ General Principles

- **Readability**: Code should be easy to understand
- **Consistency**: Follow established patterns
- **Simplicity**: Prefer simple solutions over complex ones
- **Documentation**: Document non-obvious code
- **Testing**: Write tests for all code

## 🔤 Naming Conventions

### Variables

- Use camelCase for variables and function names
- Use descriptive names that indicate purpose
- Avoid abbreviations unless they are widely understood

```typescript
// Good
const userProfile = getUserProfile(userId);

// Bad
const up = getUP(uid);
```

### Classes

- Use PascalCase for class names
- Use noun phrases for class names

```typescript
// Good
class DocumentManager {
  // ...
}

// Bad
class manage_docs {
  // ...
}
```

### Files

- Use kebab-case for file names
- Group related files in directories

```
// Good
user-service.ts
user-service.test.ts

// Bad
UserService.ts
userservicetest.ts
```

## 🧩 TypeScript Guidelines

- Use explicit types when they aren't obvious
- Prefer interfaces for object typing
- Use type guards for runtime type checking
- Avoid `any` type when possible

```typescript
// Good
interface User {
  id: string;
  name: string;
  email: string;
}

function getUserById(id: string): User | null {
  // ...
}

// Bad
function getUserById(id): any {
  // ...
}
```

## 🏗️ Architecture Patterns

- Follow the controller-service-repository pattern
- Keep controllers thin
- Put business logic in services
- Use repositories for data access

## 📝 Comments

- Comment complex logic or non-obvious decisions
- Use JSDoc for public API methods
- Don't comment obvious code

```typescript
/**
 * Fetches a user by email and verifies their access token
 * @param email - User's email address
 * @param token - Access token to verify
 * @returns The user if verification succeeds, null otherwise
 */
async function verifyUserAccess(email: string, token: string): Promise<User | null> {
  // ...
}
```

## 🧪 Testing Standards

- Write unit tests for all services and utilities
- Write integration tests for API endpoints
- Use descriptive test names that explain what is being tested

```typescript
describe('UserService', () => {
  describe('createUser', () => {
    it('should create a new user with hashed password', async () => {
      // ...
    });
    
    it('should throw an error if email already exists', async () => {
      // ...
    });
  });
});
```

## 🔍 Code Review Checklist

- Does the code follow the style guide?
- Is the code well-tested?
- Is the code efficient and performant?
- Is the code secure?
- Is the code maintainable?
```

## 🗒️ Template Sections

| Section | Purpose | Required? |
|---------|---------|-----------|
| General Principles | Overarching coding philosophy | Yes |
| Naming Conventions | Standards for naming variables, classes, etc. | Yes |
| Language-Specific Guidelines | Standards specific to the language used | Yes |
| Architecture Patterns | Patterns to follow in the codebase | Yes |
| Comments | When and how to use comments | Yes |
| Testing Standards | How to write and structure tests | Yes |
| Code Review Checklist | What to check during code reviews | Yes |

## 🧙‍♂️ Best Practices

1. **Be specific**: Provide concrete examples of good and bad practices
2. **Be realistic**: Set standards that can actually be followed
3. **Use automation**: Mention linting and formatting tools that enforce standards
4. **Explain why**: Give rationales for guidelines where appropriate
5. **Balance flexibility and consistency**: Allow for sensible exceptions to rules

## 🔄 Relationship to Company Documentation

The repository code style guide should:

- Build upon company-wide coding standards
- Adapt general principles to the specific technology stack
- Focus on patterns and practices unique to the repository
- Reference broader company standards instead of duplicating them

## 🔍 Related Documents

- [README Template](./01-readme-template.md)
- [Contributing Guide](./02-contributing-guide.md)
- [Company Code Standards](../02-engineering/02-development/07-code-style.md)
