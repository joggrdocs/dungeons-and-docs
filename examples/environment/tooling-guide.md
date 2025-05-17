# 🧰 Tooling Guide

This guide documents the tools, extensions, and configurations used for Joggr Platform development.

## 🔨 Required Tools

| Tool | Version | Purpose | Installation Guide |
|------|---------|---------|-------------------|
| Node.js | v20+ | JavaScript runtime | [Node.js Installation](https://nodejs.org/en/download/) |
| pnpm | v8+ | Package manager | [pnpm Installation](https://pnpm.io/installation) |
| Docker | v27+ | Containerization | [Docker Desktop Installation](https://docs.docker.com/desktop/install/) |

## 🧩 IDE & Extensions

### Recommended IDE

Visual Studio Code - [Download](https://code.visualstudio.com/download)

### Essential Extensions

| Extension | Purpose | Installation |
|-----------|---------|--------------|
| ESLint | JavaScript linting | Install from VS Code marketplace |
| Prettier | Code formatting | Install from VS Code marketplace |
| GitLens | Git integration | Install from VS Code marketplace |

### IDE Configuration

```json
{
  // Core settings
  "editor.formatOnSave": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  // Extension specific settings
  "prettier.singleQuote": true,
  "prettier.semi": true,
  "prettier.tabWidth": 2,
  "prettier.printWidth": 100
}
```

## 🔄 Git Hooks

| Hook | Purpose | Configuration |
|------|---------|---------------|
| pre-commit | Lint and format code | Configured via husky and lint-staged |
| commit-msg | Enforce conventional commits | Configured via commitlint |

## 🧪 Testing Tools

| Tool | Purpose | Configuration |
|------|---------|---------------|
| Jest | Unit testing | Configured in jest.config.js |
| Cypress | E2E testing | Configured in cypress.config.js |

## 🔍 Related Documents

- [Local Setup Guide](../project/setup-local-environment.md)
- [Code Style Standards](../standards/code-style.md)
- [Testing Standards](../standards/testing.md)

## 📚 Additional Resources

- [Official Node.js Documentation](https://nodejs.org/en/docs/)
- [Official pnpm Documentation](https://pnpm.io/motivation)
- [Joggr Tool Configuration Repo](https://github.com/joggrdocs/tooling)
