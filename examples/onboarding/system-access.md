# 🔐 System Access Guide

This guide provides instructions for gaining access to all the systems, tools, and repositories you'll need for your quests at Joggr.

## 🗝️ Core Systems

| System | Purpose | Access Request Process | Owner |
|--------|---------|------------------------|-------|
| Joggr Platform | Main documentation platform | Submit request via IT portal | Platform Team |
| GitHub | Code repository and version control | Submit request via IT portal | DevOps Team |
| AWS Console | Cloud infrastructure management | Submit request via IT portal with manager approval | Infrastructure Team |

## 💻 Development Tools

| Tool | Purpose | Installation Instructions | 
|------|---------|---------------------------|
| VS Code | Primary IDE | Download from [VS Code website](https://code.visualstudio.com/) and install | 
| Node.js | JavaScript runtime | Use nvm: `nvm install 20` and `nvm use 20` |
| Docker | Containerization | Follow [Docker Desktop installation guide](https://docs.docker.com/desktop/install/) |

## 📦 Repositories

| Repository | Description | Access Level Needed | How to Request |
|------------|-------------|---------------------|----------------|
| joggrdocs/platform | Main platform codebase | Developer | Request via GitHub team in IT portal |
| joggrdocs/api | API service | Developer | Request via GitHub team in IT portal |
| joggrdocs/infrastructure | Infrastructure as code | Read-only | Request via Infrastructure team |

## 🌐 Environments

| Environment | Purpose | URL | Access Level |
|-------------|---------|-----|-------------|
| Development | Feature development and testing | https://dev.joggr.io | Full access for all developers |
| Staging | Pre-production testing | https://staging.joggr.io | Read/write for developers |
| Production | Live environment | https://app.joggr.io | Read-only for most developers, write for release managers |

## 🛡️ Security Policies

1. All production credentials must be stored in AWS Secrets Manager, never in code or local files
2. MFA is required for all system access
3. Access reviews are conducted quarterly to ensure proper permission levels

## 🔍 Related Documents

- [Welcome Guide](./welcome-guide.md)
- [Development Environment Setup](../environment/setup-guide.md)
- [Security Standards](../security/security-standards.md)

## 📚 Additional Resources

- [IT Support Portal](https://it.joggr.io)
- [Security Handbook](https://security.joggr.io)
- [Access Request Form](https://it.joggr.io/access-request)
