<!--  
�� Usage:  
- Replace all {{placeholders}} with your organization's content
- Update links and remove unnecessary sections
- Customize as needed 

Happy documenting! 🚀  
-->

# 🏗️ Service Architecture

This document provides an overview of the services, vendors, and assets that make up the {{ app }} platform and how they interact.

## 🎯 Core Services

| Service | Description | Endpoint | Owner |
|---------|-------------|----------|-------|
| 🔌 **API** | The {{ app }} **API** is the main API for our Platform. It is responsible for all of the business logic and data storage for the Platform. | `{{ api-endpoint }}` | {{ api-owner }} |
| 🌐 **Web** | The {{ app }} **Web** consists of a React-based application that is a SPA. | `{{ web-endpoint }}` | {{ web-owner }} |
| ⚙️ **Server** | The {{ app }} **Server** is a Fastify based API that serves the **Web** to the client. | `{{ server-endpoint }}` | {{ server-owner }} |
| 🔗 **Third-Party Service** | The {{ app }} **Third-Party Service** is a proxy API for {{ third-party-reason }}. | `{{ third-party-endpoint }}` | {{ third-party-owner }} |

## 🔄 System Flow

```mermaid
%%{init: {
  'theme': 'default',
  'themeVariables': {
    'primaryColor': '#f4f4f4',
    'primaryTextColor': '#333',
    'primaryBorderColor': '#888',
    'lineColor': '#555',
    'secondaryColor': '#eee',
    'tertiaryColor': '#fff'
  }
}}%%

flowchart TD
    %% Title
    title["{{ company-name }} Service Architecture"]
    style title fill:none,stroke:none,color:#333,font-weight:bold

    %% Core Services
    web("🌐 Web Client")
    style web fill:#7b1fa2,color:white,stroke:#5d1777,stroke-width:2px

    api("⬆️ Backend API")
    style api fill:#7b1fa2,color:white,stroke:#5d1777,stroke-width:2px

    server("💻 Web Server")
    style server fill:#7b1fa2,color:white,stroke:#5d1777,stroke-width:2px

    third-party("🐙 Third-Party Proxy")
    style third-party fill:#00897b,color:white,stroke:#005b4f,stroke-width:2px

    %% Database Services
    database[("🐘 {{ database-name }}")]
    style database fill:#0064a5,color:white,stroke:#004c7f,stroke-width:2px

    bucket("🪣 Storage Bucket")
    style bucket fill:#0064a5,color:white,stroke:#004c7f,stroke-width:2px

    %% Vendor Services
    auth("🔐 {{ auth-provider }}")
    style auth fill:#f57c00,color:white,stroke:#bc5100,stroke-width:2px

    thirdpartyapi("🔌 {{ third-party-api }}")
    style thirdpartyapi fill:#f57c00,color:white,stroke:#bc5100,stroke-width:2px

    %% Connections
    web -- "Serves UI" --> server
    web <-- "API Requests" --> api
    web <-- "CDN Assets" --> api
    api <-- "Static Assets" --> bucket
    api <-- "Auth" --> auth
    web <-- "Login" --> auth
    third-party <-- "Proxy Requests" --> thirdpartyapi
    api -- "Database Queries" --> database

    %% Network Groups
    subgraph vpc ["🛜 VPC Network"]
        direction TB
        api -- "Internal API Calls" --> third-party
        server
        api
    end
    style vpc fill:#e3f2fd,color:#0d47a1,stroke:#0d47a1,stroke-width:3px,stroke-dasharray:5

    subgraph cloud ["💽 {{ cloud-provider }} Managed Services"]
        direction TB
        database
        bucket
    end
    style cloud fill:#e1f5fe,color:#01579b,stroke:#01579b,stroke-width:3px,stroke-dasharray:5

    subgraph vendors ["🏪 External Vendors"]
        direction TB
        thirdpartyapi
        auth
    end
    style vendors fill:#fff3e0,color:#e65100,stroke:#e65100,stroke-width:3px,stroke-dasharray:5

    %% Global link styling
    linkStyle default stroke-width:2px,stroke:#666
```

## 🔒 Security

### Authentication
- {{ auth-provider }} for user authentication
- {{ auth-flow-description }}

### Authorization
- {{ authorization-model }}
- {{ role-descriptions }}

## 📊 Monitoring & Observability

### Metrics
- {{ metric-1 }}
- {{ metric-2 }}
- {{ metric-3 }}

### Logging
- {{ logging-tool }}
- {{ log-retention-policy }}

## 🔍 Related Documents

- [Infrastructure Overview](./infrastructure.md)
- [Security Standards](./security.md)
- [Deployment Process](./deployment.md)

## 📚 Additional Resources

- [{{ app }} Architecture Decisions](../architecture/decisions.md)
- [Service Dependencies](./dependencies.md)
- [Performance Guidelines](./performance.md)
