# 🧰 Tooling Guide

This guide documents the tools, extensions, and configurations used for Spellforge Codex development.

## 🔨 Required Tools

| Tool | Version | Purpose | Installation Guide |
|------|---------|---------|-------------------|
| Node.js | v20+ | JavaScript runtime | [Node.js Installation](https://nodejs.org/en/download/) |
| pnpm | v8+ | Package manager | [pnpm Installation](https://pnpm.io/installation) |
| Docker | v27+ | Containerization | [Docker Desktop Installation](https://docs.docker.com/desktop/install/) |
| Git | Latest | Version control | [Git Installation](https://git-scm.com/downloads) |
| VS Code | Latest | IDE | [VS Code Installation](https://code.visualstudio.com/download) |

## 🧩 IDE & Extensions

### Recommended IDE

Visual Studio Code - [Download](https://code.visualstudio.com/download)

### Essential Extensions

| Extension | Purpose | Installation |
|-----------|---------|--------------|
| ESLint | JavaScript linting | Install from VS Code marketplace |
| Prettier | Code formatting | Install from VS Code marketplace |
| GitLens | Git integration | Install from VS Code marketplace |
| Docker | Docker management | Install from VS Code marketplace |
| Jest Runner | Running tests | Install from VS Code marketplace |

### IDE Configuration

```json
{
  // Core settings
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  // Extension specific settings
  "prettier.singleQuote": true,
  "prettier.semi": true,
  "prettier.tabWidth": 2,
  "prettier.printWidth": 100,
  "eslint.validate": ["javascript", "typescript", "typescriptreact"],
  "typescript.tsdk": "node_modules/typescript/lib"
}
```

## 🔄 Git Hooks

| Hook | Purpose | Configuration |
|------|---------|---------------|
| pre-commit | Lint and format code | Configured via husky and lint-staged |
| commit-msg | Enforce conventional commits | Configured via commitlint |
| pre-push | Run tests | Configured via husky |

## 🧪 Testing Tools

| Tool | Purpose | Configuration |
|------|---------|---------------|
| Jest | Unit testing | Configured in jest.config.js |
| React Testing Library | Component testing | Used with Jest |
| Cypress | E2E testing | Configured in cypress.config.js |
| Playwright | Browser testing | Configured in playwright.config.js |

## 📊 Monitoring & Debugging

| Tool | Purpose | Access |
|------|---------|--------|
| Datadog | Application monitoring | [Datadog Dashboard](https://app.datadoghq.com) |
| Sentry | Error tracking | [Sentry Dashboard](https://sentry.io) |
| Lighthouse | Performance monitoring | Built into Chrome DevTools |
| React DevTools | React debugging | Browser extension |

## 🔍 Related Documents

- [Development Environment Setup](./01-setup-guide.md)
- [Repository Structure](./03-repo-structure.md)
- [Code Style Standards](../02-development/07-code-style.md)
- [Testing Strategy](../03-testing/01-testing-strategy.md)

## 📚 Additional Resources

- [Official Node.js Documentation](https://nodejs.org/en/docs/)
- [Official pnpm Documentation](https://pnpm.io/motivation)
- [VS Code Shortcuts](https://code.visualstudio.com/docs/getstarted/keybindings)
- [Spellforge Tool Configuration Repo](https://github.com/spellforge/tooling)
