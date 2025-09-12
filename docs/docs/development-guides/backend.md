---
sidebar_position: 2
---

# Backend

The backend uses **Node.js** with **Express**.

### Setup

```
cd backend
npm install
npm run dev       # or npm run dev:ts if using ts-node-dev
```
The server should be running at http://localhost:8080.

### Testing

```
npm test
```
Tests are located in backend/tests.

### Linting & Formatting

```
npm run lint
npm run format
```

### Best Practices
- Follow RESTful route conventions.
- Keep services stateless.
- Use environment variables for configuration (.env).
- Write unit tests for controllers and services.