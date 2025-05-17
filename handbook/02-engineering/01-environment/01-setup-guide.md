# ⚙️ Development Environment Setup

This arcane guide will help you set up your development environment for contributing to Spellforge's magical projects.

## 🧙‍♂️ Requirements

* 🐳 [Docker v27+](https://docs.docker.com/desktop/install/) (installed via Docker Desktop)
* 🟢 [Node.js v20+](https://nodejs.org/en/download) (we recommend using nvm)
* 📦 [pnpm v8+](https://pnpm.io/installation) (our preferred package manager)
* 📟 [Git](https://git-scm.com/downloads) (for version control)

## 🚀 Getting Started

### 🔹 Step 1: Clone the repository

Clone the Codex repository to your local machine.

```shell
git clone https://github.com/spellforge/codex.git
cd codex
```

### 🔹 Step 2: Install dependencies

Install the project dependencies using pnpm.

```shell
pnpm install
```

### 🔹 Step 3: Set up environment variables

Copy the example environment file and update it with your local settings.

```shell
cp .env.example .env.local
```

Edit `.env.local` and update the following variables:

```
DATABASE_URL=postgresql://postgres:postgres@localhost:5432/codex
API_KEY=local-development-key
```

### 🔹 Step 4: Start the development environment

Start the development environment using Docker Compose.

```shell
docker-compose up -d
```

### 🔹 Step 5: Run database migrations

Run the database migrations to set up your local database.

```shell
pnpm db:migrate
```

### 🔹 Step 6: Start the development server

Start the development server.

```shell
pnpm dev
```

## 🎉 Done

You are all set and ready to cast your first development spell! You can now view the running app at: `http://localhost:3000`

## 🧩 Project Structure

```
codex/
├── apps/                # Applications
│   ├── web/             # Frontend web application
│   └── api/             # Backend API service
├── packages/            # Shared packages
│   ├── ui/              # UI component library
│   ├── config/          # Shared configurations
│   └── utils/           # Shared utilities
├── docs/                # Documentation
├── scripts/             # Development scripts
└── docker/              # Docker configurations
```

## 🛠️ Troubleshooting

* **Database Connection Error**: Make sure Docker is running and the database container is up. Check with `docker-compose ps`.

* **Node.js Version Error**: Make sure you're using Node v20+. If using nvm, run `nvm use 20`.

* **Port Conflict**: If port 3000 is already in use, you can change the port in the `.env.local` file by setting `PORT=3001`.

* **Docker Issues**: If you encounter Docker-related issues, try running `docker-compose down -v` followed by `docker-compose up -d` to recreate the containers.

## 🔍 Related Documents

- [Tooling Guide](./02-tooling-guide.md)
- [Repository Structure](./03-repo-structure.md)
- [Local Development Workflow](../02-development/05-development-workflow.md)
- [Secrets Management](./04-secrets-management.md)

## 📚 Additional Resources

- [Docker Documentation](https://docs.docker.com/)
- [Node.js Documentation](https://nodejs.org/en/docs/)
- [pnpm Documentation](https://pnpm.io/motivation)
- [Git Workflow](../02-development/06-git-workflow.md)
