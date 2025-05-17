# 🔐 System Access Guide

This guide provides instructions for gaining access to all the systems, tools, and repositories you'll need for your quests at Spellforge Technologies.

## 🗝️ Core Systems

| System | Purpose | Access Request Process | Owner |
|--------|---------|------------------------|-------|
| GitHub | Code repository | Added by Engineering Manager upon onboarding | Engineering Operations |
| Codex Platform | Our main product | Self-service with company email | Product Team |
| 1Password | Secrets management | Added by IT upon onboarding | Security Team |
| Slack | Team communication | Added by HR upon onboarding | HR Team |
| Linear | Issue tracking | Added by Engineering Manager upon onboarding | Engineering Operations |
| AWS Console | Cloud infrastructure | Request via IT ticket with manager approval | DevOps Team |

## 💻 Development Tools

| Tool | Purpose | Installation Instructions | 
|------|---------|---------------------------|
| Node.js | JavaScript runtime | Use nvm: `nvm install 20` | 
| pnpm | Package manager | `npm install -g pnpm` |
| Docker | Containerization | [Docker Desktop Installation](https://docs.docker.com/desktop/install/) |
| VS Code | IDE | [Download](https://code.visualstudio.com/download) |
| Postman | API testing | [Download](https://www.postman.com/downloads/) |

## 📦 Repositories

| Repository | Description | Access Level Needed | How to Request |
|------------|-------------|---------------------|----------------|
| spellforge/codex | Main product codebase | Developer | Added automatically |
| spellforge/arcane-api | Backend API | Developer | Added automatically |
| spellforge/spellbook-ui | Component library | Developer | Added automatically |
| spellforge/infrastructure | IaC templates | DevOps Access | Request via IT ticket |
| spellforge/design-system | Design system | Developer | Added automatically |

## 🌐 Environments

| Environment | Purpose | URL | Access Level |
|-------------|---------|-----|-------------|
| Local | Development | localhost | Full access |
| Development | Integration testing | https://dev.spellforge.tech | Full access |
| Staging | Pre-production testing | https://staging.spellforge.tech | Read/Write |
| Production | Live environment | https://app.spellforge.tech | Read-only (deploy via CI) |

## 🛡️ Security Policies

1. Use 1Password for all credentials, never share secrets through Slack
2. Enable 2FA for all services
3. Follow the principle of least privilege - only request access you need
4. Report security incidents immediately to security@spellforge.tech
5. Lock your computer when away from your desk, even in remote settings

## 🔍 Related Documents

- [Welcome Guide](./01-welcome-guide.md)
- [Development Environment Setup](../../02-engineering/01-environment/01-setup-guide.md)
- [Security Standards](../../04-security/01-standards/01-security-standards.md)
- [Glossary of Terms](./03-glossary.md)

## 📚 Additional Resources

- [IT Support Portal](https://help.spellforge.tech)
- [Security Handbook](https://security.spellforge.tech)
- [Access Request Form](https://access.spellforge.tech)
