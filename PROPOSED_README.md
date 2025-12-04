# 🚀 Apex-NodeJS-Express-WebApp-Boilerplate

**Apex NodeJS Express WebApp Boilerplate** is a meticulously engineered, production-grade starter kit designed for hyper-accelerated development of robust backend services using the Express framework. It formalizes infrastructure patterns, including comprehensive Dockerization and out-of-the-box integration hooks for GitHub Codespaces, ensuring a zero-configuration path from concept to deployment.

---

## 📜 Agent Directives & System Integrity (December 2025 Standard)

<details>
<summary><strong>🤖 APEX ARCHITECT CONTEXT & VERIFICATION PROTOCOL</strong></summary>

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** Senior Principal Software Architect, 40+ years experience. Enforcing FAANG-level standards.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."
**Output Standard:** EXECUTION-ONLY.

### 2. INPUT PROCESSING & COGNITION (NODE/EXPRESS CONTEXT)
*   **Technology Anchor:** This repository is anchored in the **Node.js/Express Ecosystem** (LTS, targetting Node 22+). All architectural decisions must align with modern asynchronous patterns.
*   **MANDATORY MCP INSTRUMENTATION (Node/EJS Stack Verification):**
    *   **No Guessing:** Do not hallucinate missing dependencies or configuration files.
    *   **Research First:** Use `linkup`/`brave` to search for **Latest Express Security Patches (Q4 2025)** and **EJS/Tailwind (if applicable) performance benchmarks**.
    *   **Validation:** Use `docfork` to verify all **`package.json` dependency signatures** against known vulnerabilities.
    *   **Reasoning:** Engage `clear-thought-two` to architect load-balancing or container orchestration patterns *before* modifying Dockerfiles.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
*   **PRIMARY SCENARIO: WEB / API (NodeJS/Express)**
    *   **Stack:** **Node.js 22+ (LTS)**, **Express.js 5.x** (Mandatory adherence to Express 5 best practices), **TypeScript (Strict)** for core service logic (even if EJS templating is used on the surface), **Biome** (for unified linting/formatting speed), **Vitest** (for unit testing), **Playwright** (for E2E/Integration). EJS remains for server-side rendering views.
    *   **Architecture:** Enforce a **Feature-Sliced Design (FSD)** pattern adapted for the backend (e.g., `features/`, `entities/`, `shared/`). All routes must pass through centralized middleware stacks.
    *   **Containerization:** Docker configurations optimized for multi-stage builds, targeting minimal image sizes using Alpine/Distroless bases where possible.

### 4. VERIFICATION & DEPLOYMENT COMMANDS (Node/Express)
*   **Setup:** `npm ci` (Use `npm ci` exclusively for reproducible builds).
*   **Lint/Format Check:** `npx @biomejs/biome check .`
*   **Test Execution:** `npx vitest run` (Unit) & `npx playwright test` (E2E).
*   **Container Build:** `docker build -t boilerplate .`

</details>

--- 

## 🏗️ Architectural Blueprint

This boilerplate enforces structural discipline vital for scaling beyond the initial prototype phase.

ascii
/Apex-NodeJS-Express-WebApp-Boilerplate
├── .github/                   # CI/CD, Templates, Security
├── src/
│   ├── config/                # Environment configuration loaders (Zod validation recommended)
│   ├── controllers/           # Request handling logic (Thin layer)
│   ├── features/              # FSD implementation: Business Logic Modules (Core of application)
│   ├── middleware/            # Global and specific request processing pipelines
│   ├── models/                # Data structure definitions (e.g., Mongoose schemas, TypeScript interfaces)
│   └── views/                 # EJS Templates (Server-Side Rendering)
├── Dockerfile                 # Multi-stage build for production readiness
├── package.json
└── README.md


## 🧭 Development & Verification

Follow these steps immediately after cloning to establish environment parity and verify integrity.

1.  **Clone & Initialize:**
    bash
    git clone https://github.com/chirag127/Apex-NodeJS-Express-WebApp-Boilerplate.git
    cd Apex-NodeJS-Express-WebApp-Boilerplate
    npm ci
    

2.  **Local Execution (Development Mode):**
    bash
    npm run dev
    # Server typically starts on http://localhost:3000
    

3.  **Integrity Verification (Linter & Tests):**
    bash
    # Run Biome static analysis (Linting and Formatting)
    npm run lint

    # Execute Unit Tests
    npm run test:unit

    # Execute End-to-End Tests using Playwright
    npm run test:e2e
    

### Scripts Reference Table

| Script | Command | Description |
| :--- | :--- | :--- |
| `start` | `node dist/index.js` | Production server start (assuming compiled TS/JS output) |
| `dev` | `npm run watch & npm run start:dev` | Development server with watch mode |
| `build` | `npm run build:ts` | Compile TypeScript source to JavaScript |
| `lint` | `npx @biomejs/biome check .` | Run code quality and formatting checks |
| `test:unit` | `npx vitest run` | Run application unit tests |

## 🏛️ Guiding Architectural Principles

This project is architected strictly around established paradigms:

*   **SOLID:** Ensures modularity and maintainability within feature modules.
*   **DRY (Don't Repeat Yourself):** Centralized configuration and middleware layers prevent code duplication.
*   **YAGNI (You Ain't Gonna Need It):** Features are deliberately scoped to a minimum viable architecture, avoiding premature complexity.

