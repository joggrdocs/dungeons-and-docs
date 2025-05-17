# 🔒 Secrets & Configuration Management

This guide outlines how to properly manage secrets, environment variables, and configuration across different environments for Joggr Platform.

## 🎯 Core Principles

1. **Never commit secrets** to version control
2. **Use environment-specific configurations** for different environments
3. **Least privilege access** to secrets and configurations

## 🗝️ Secret Storage

| Environment | Storage Solution | Access Method | Owner |
|-------------|-----------------|---------------|-------|
| Development | .env.local files | Local file, not committed | Individual Developer |
| Staging | AWS Secrets Manager | AWS CLI or SDK with IAM role | DevOps Team |
| Production | AWS Secrets Manager | AWS CLI or SDK with IAM role | Security Team |

## 🔄 Configuration Management

### Environment Variables

```dotenv
# Required variables
DATABASE_URL=postgresql://user:password@localhost:5432/joggr
API_KEY=your-api-key-here

# Optional variables
DEBUG=false
LOG_LEVEL=info
```

### Configuration Files

| File | Purpose | Template Location |
|------|---------|-------------------|
| .env.example | Template for local environment variables | [Repository Root](https://github.com/joggrdocs/joggr-platform) |
| config.js | Runtime configuration | [Config Directory](https://github.com/joggrdocs/joggr-platform/tree/main/config) |

## 🛡️ Security Best Practices

1. **Rotation Schedule**
   - Production secrets are rotated every 90 days
   - API keys are rotated every 30 days
   - Database credentials are rotated every 60 days

2. **Access Control**
   - Only DevOps and Security teams have access to production secrets
   - Staging environment secrets are accessible to all developers
   - Local environment secrets are managed by individual developers

3. **Auditing**
   - All secret access is logged and monitored
   - Quarterly access reviews are conducted
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
```

## 🔍 Related Documents

- [Local Setup Guide](../project/setup-local-environment.md)
- [Deployment Guide](../project/deployment-guide.md)
- [Security Standards](../security/security-standards.md)

## 📚 Additional Resources

- [AWS Secrets Manager Documentation](https://docs.aws.amazon.com/secretsmanager/)
- [Environment Variable Best Practices](https://12factor.net/config)
- [Security Handbook](https://security.joggr.io)
