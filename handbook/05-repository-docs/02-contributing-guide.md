# 🤝 Repository Contributing Guide Template

This document provides a template for CONTRIBUTING.md files in Spellforge Technologies repositories.

## ✨ Example CONTRIBUTING.md

```markdown
# 🤝 Contributing to Arcane API

Thank you for your interest in contributing to the Arcane API! This guide will help you get started with the development process.

## 🧙‍♂️ Code of Conduct

Please review our [Code of Conduct](https://docs.spellforge.tech/code-of-conduct) before contributing.

## 🌱 Getting Started

1. **Fork the repository**
2. **Clone your fork**
   ```bash
   git clone https://github.com/your-username/arcane-api.git
   cd arcane-api
   ```
3. **Install dependencies**
   ```bash
   pnpm install
   ```
4. **Set up environment**
   ```bash
   cp .env.example .env.local
   ```
5. **Create a branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```

## 🧪 Development Process

1. **Make your changes**
2. **Write tests** for your changes
3. **Run linting**
   ```bash
   pnpm lint
   ```
4. **Run tests**
   ```bash
   pnpm test
   ```
5. **Commit your changes** using [Conventional Commits](https://www.conventionalcommits.org/)
   ```bash
   git commit -m "feat: add amazing feature"
   ```
6. **Push to your fork**
   ```bash
   git push origin feature/amazing-feature
   ```
7. **Create a Pull Request**

## 📋 Pull Request Guidelines

- Fill out the PR template completely
- Link to any relevant issues
- Include screenshots or recordings for UI changes
- Make sure all tests pass
- Get at least one code review before merging

## 🏗️ Project Structure

```
arcane-api/
├── src/               # Source code
│   ├── controllers/   # Request handlers
│   ├── middleware/    # Express middleware
│   ├── models/        # Data models
│   ├── routes/        # API routes
│   ├── services/      # Business logic
│   └── utils/         # Utility functions
├── prisma/            # Database schema
├── tests/             # Test files
├── scripts/           # Utility scripts
└── config/            # Configuration files
```

## 🧠 Style Guide

We follow the [Spellforge TypeScript Style Guide](https://docs.spellforge.tech/style-guide).

## 📚 Additional Resources

- [API Documentation](https://docs.spellforge.tech/api)
- [Architecture Overview](https://docs.spellforge.tech/architecture)
- [TypeScript Style Guide](https://docs.spellforge.tech/style-guide)
```

## 🗒️ Template Sections

| Section | Purpose | Required? |
|---------|---------|-----------|
| Introduction | Welcomes contributors | Yes |
| Code of Conduct | Sets behavioral expectations | Yes |
| Getting Started | First steps for new contributors | Yes |
| Development Process | Step-by-step contribution workflow | Yes |
| Pull Request Guidelines | Expectations for PRs | Yes |
| Project Structure | Overview of codebase organization | Yes |
| Style Guide | Coding standards | Yes |
| Additional Resources | Links to related documentation | Yes |

## 🧙‍♂️ Best Practices

1. **Be welcoming**: Encourage contributions from everyone
2. **Be clear**: Provide explicit instructions for contribution workflow
3. **Be helpful**: Include troubleshooting information for common issues
4. **Be consistent**: Align with company-wide processes while highlighting repo-specific details
5. **Keep updated**: Ensure the guide reflects the current state of the project

## 🔄 Relationship to Company Documentation

The repository CONTRIBUTING.md should:

- Focus on repository-specific contribution processes
- Reference company-wide standards and guidelines
- Provide clear links to broader documentation
- Emphasize unique aspects of the particular repository

## 🔍 Related Documents

- [README Template](./01-readme-template.md)
- [Code Style Guide](./03-code-style-guide.md)
- [Pull Request Template](./04-pr-template.md)
- [Development Workflow](../02-engineering/02-development/05-development-workflow.md)
