---
sidebar_position: 7
sidebar_label: Project Structure
---

# Project Structure

Our project uses a **monorepo** to manage multiple of the software application which work together to achieve the goal of the project. This approach ensures consistency, centralisation, simplifies dependency management, and allows seamless collaboration across teams.

The monorepo is organised to support scalability, maintainability, and ease of development.

```
root/
├── frontend/               # React or web UI
│   ├── public/             # Static assets (images, favicon, etc.)
│   ├── src/                # Source code (components, pages, utils)
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── context/
│   │   └── utils/
│   ├── tests/              # Unit/integration tests for frontend
│   ├── package.json
│   ├── tsconfig.json
│   └── README.md
│
├── backend/                # Node.js + Express (or other backend framework)
│   ├── src/
│   │   ├── controllers/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── middleware/
│   │   └── utils/
│   ├── tests/              # Unit/integration tests for backend
│   ├── package.json
│   ├── tsconfig.json
│   └── README.md
│
├── db/                     # Database schema, migrations, seeders
│   ├── migrations/
│   ├── seeders/
│   ├── schema/             # SQL or ORM models
│   ├── scripts/            # DB setup scripts
│   └── README.md
│
├── shared/                 # Shared code across frontend & backend
│   ├── constants/
│   ├── types/              # TypeScript interfaces/types
│   ├── utils/
│   └── README.md
│
├── docs/                   # Docusaurus or markdown docs
│   ├── static/             # Images, assets for docs
│   ├── src/                # Markdown files, Docusaurus config
│   ├── docusaurus.config.js
│   └── README.md
│
├── .gitignore
├── package.json            # Root-level scripts, e.g., build, lint, test
├── tsconfig.base.json      # Base TypeScript config for frontend & backend
├── lerna.json / pnpm-workspace.yaml / turbo.json  # Monorepo tool config
└── README.md
```