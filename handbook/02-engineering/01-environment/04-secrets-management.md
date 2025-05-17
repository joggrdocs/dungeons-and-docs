# 🔒 Secrets & Configuration Management

This guide outlines how to properly manage secrets, environment variables, and configuration across different environments for Spellforge Codex.

## 🎯 Core Principles

1. **Never commit secrets** to version control
2. **Use environment-specific configurations** for different environments
3. **Least privilege access** to secrets and configurations
4. **Rotate secrets** regularly
5. **Audit access** to sensitive information

## 🗝️ Secret Storage

| Environment | Storage Solution | Access Method | Owner |
|-------------|-----------------|---------------|-------|
| Development | .env.local files | Local file, not committed | Individual Developer |
| Staging | AWS Secrets Manager | CI/CD pipeline, IAM roles | DevOps Guild |
| Production | AWS Secrets Manager | CI/CD pipeline, IAM roles | DevOps Guild |

## 🔄 Configuration Management

### Environment Variables

```dotenv
# Required variables
DATABASE_URL=postgresql://user:password@localhost:5432/codex
API_KEY=your-api-key

# Optional variables
DEBUG=false
LOG_LEVEL=info
```

### Configuration Files

| File | Purpose | Template Location |
|------|---------|-------------------|
| .env.example | Template for local environment variables | Root of repository |
| config/default.js | Default configuration values | config/ directory |
| config/production.js | Production-specific overrides | config/ directory |

## 🛡️ Security Best Practices

1. **Rotation Schedule**
   - Production secrets: Rotated every 90 days
   - API keys: Rotated every 180 days
   - Access credentials: Rotated when team members leave

2. **Access Control**
   - Production secrets: Limited to DevOps Guild and Engineering Leads
   - Staging secrets: Available to all Engineers
   - Development secrets: Managed by individual developers

3. **Auditing**
   - All secret access is logged and monitored
   - Regular audits of secret access are conducted quarterly
   - Anomalous access patterns trigger alerts

## 🚀 Local Development

```shell
# Clone the env template
cp .env.example .env.local

# Fill in the required values
# NEVER commit .env.local to version control

# Load the environment variables
source .env.local  # Unix/Linux
# OR
# Use the provided script for Windows
./scripts/load-env.ps1
```

## 🧙‍♂️ Accessing Secrets in Code

### Node.js

```javascript
// Using dotenv
require('dotenv').config();

// Accessing environment variables
const apiKey = process.env.API_KEY;

// Using config package for structured configuration
const config = require('config');
const dbConfig = config.get('database');
```

### React

```javascript
// Environment variables in React must be prefixed with REACT_APP_
const apiUrl = process.env.REACT_APP_API_URL;
```

## 🔍 Related Documents

- [Development Environment Setup](./01-setup-guide.md)
- [Deployment Guide](../../03-operations/02-deployment/01-deployment-guide.md)
- [Security Standards](../../04-security/01-standards/01-security-standards.md)
- [Infrastructure Overview](../../03-operations/01-infrastructure/01-infrastructure-overview.md)

## 📚 Additional Resources

- [AWS Secrets Manager Documentation](https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html)
- [Environment Variable Best Practices](https://12factor.net/config)
- [Security Handbook](https://security.spellforge.tech)
