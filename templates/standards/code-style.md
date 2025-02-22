<!--  
📝 Usage:  
- Replace *placeholders* with relevant details.  
- Update links and remove unnecessary sections.  
- Customize as needed.  

Happy documenting! 🚀  
-->

# 👨‍💻 Code Standards

As an engineering organization focused on operational excellence, we understand that the code itself many times is the best documentation and keeping a standardized format for things like file naming, function declarations, and more, is important for the end-reader of code. This includes when trying to review code, decipher code you didn't write or pulling in samples. We live by one rule with our code styles:

> You cannot tell who wrote the code, only that someone on the {{team-name}} did.

## Coding Standards

### Naming Conventions

**Variables & Functions:** `camelCase`

```typescript
const userName = 'JohnDoe';
function getUserData() {
  // function logic
}
```

**Classes & Components:** `PascalCase`

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

**Constants:** `UPPER_CASE`

```typescript
const API_KEY = '12345-ABCDE';
const MAX_USERS = 100;
```

**File Names:** `kebab-case`

```typescript
user-profile.js
dashboard-view.tsx
```

### Comments

* **Use JSDoc** for documenting functions and APIs.

* **Header Comments** for large files only.

* **Section & Subsection Comments** for organizing large logic blocks.

* **Avoid redundant comments** – describe intent, not obvious functionality.

### Linting & Formatting

* **Linting:** [ESLint](https://eslint.org/).

* **Formatting:** [Prettier](https://prettier.io/), standard config.

* **No additional warnings in PRs** – aim for zero lint errors.

### Prettier Config

```plaintext
{
  "printWidth": 80,
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true,
  "trailingComma": "es5",
  "arrowParens": "always"
}
```

### Prettier Ignore

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
