# Express-Kickstart-NodeJS-Web-App-Template

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/Express-Kickstart-NodeJS-Web-App-Template/ci.yml?style=flat-square)](https://github.com/chirag127/Express-Kickstart-NodeJS-Web-App-Template/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/Express-Kickstart-NodeJS-Web-App-Template?style=flat-square)](https://codecov.io/gh/chirag127/Express-Kickstart-NodeJS-Web-App-Template)
[![Language](https://img.shields.io/github/languages/top/chirag127/Express-Kickstart-NodeJS-Web-App-Template?style=flat-square)](https://github.com/chirag127/Express-Kickstart-NodeJS-Web-App-Template)
[![License](https://img.shields.io/github/license/chirag127/Express-Kickstart-NodeJS-Web-App-Template?style=flat-square)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/Express-Kickstart-NodeJS-Web-App-Template?style=flat-square)](https://github.com/chirag127/Express-Kickstart-NodeJS-Web-App-Template)

[⭐ Star this Repo](https://github.com/chirag127/Express-Kickstart-NodeJS-Web-App-Template)

---

## ⚡ BLUF (Bottom Line Up Front)

This repository is a zero-dependency, production-hardened boilerplate template designed for building robust web applications using Node.js, the Express framework, and EJS for templating. It provides a modern, secure foundation optimized for rapid prototyping and seamless deployment, especially within containerized environments like Docker and Codespaces.

## 🏛️ Architecture Overview

This project adheres to a **Layered (N-Tier) Architecture** for clear separation of concerns, prioritizing stability over micro-service complexity for rapid development. The EJS views sit atop a standard Express routing layer which communicates with dedicated Service and Data Access layers.

ascii
┌───────────────────────────┐
│      Client Browser       │
└────────────┬──────────────┘
             │ (HTTP/HTTPS)
┌────────────▼──────────────┐
│       Web Layer (Express)   │
│    (Routes, Middleware)     │
└────────────┬──────────────┘
             │
┌────────────▼──────────────┐
│    Service Layer (Business Logic)│
│ (Validation, Orchestration) │
└────────────┬──────────────┘
             │
┌────────────▼──────────────┐
│ Data Access Layer (DAL)   │
│ (DB Abstraction/Mongoose)   │
└────────────┴──────────────┘


## 📚 Table of Contents

1.  [⚡ BLUF (Bottom Line Up Front)](#-bluf-bottom-line-up-front)
2.  [🏛️ Architecture Overview](#-architecture-overview)
3.  [📚 Table of Contents](#-table-of-contents)
4.  [✨ Core Features](#-core-features)
5.  [🤖 AI Agent Directives (Read First)](#-ai-agent-directives-read-first)
6.  [🚀 Getting Started](#-getting-started)
    *   [Prerequisites](#prerequisites)
    *   [Installation & Setup](#installation--setup)
    *   [Development Scripts](#development-scripts)
7.  [🛡️ Development Principles](#-development-principles)
8.  [🤝 Contribution Guidelines](#-contribution-guidelines)
9.  [📄 License](#-license)

## ✨ Core Features

*   **Express/EJS Stack:** Stable, proven foundation for server-side rendered applications.
*   **Production-Ready Middleware:** Includes essential setup for security (Helmet), request logging (Morgan), and CORS handling.
*   **Docker Integration:** Pre-configured `Dockerfile` and `.dockerignore` for containerization.
*   **Codespaces Optimized:** `.devcontainer/` structure ensuring instant, standardized setup in GitHub Codespaces.
*   **ESLint & Prettier (Biome):** Linting and formatting enforced via Biome for high code quality.
*   **CI/CD:** Integrated GitHub Actions workflow for automated testing and validation upon push/PR.

## 🤖 AI Agent Directives (Read First)

<details>
<summary>Click to view **APEX Architectural Alignment & Verification Guide**</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** This repository, `Express-Kickstart-NodeJS-Web-App-Template`, is a foundational **Node.js/Express/EJS Web Application Template**.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs. If a database abstraction layer is used (e.g., Mongoose), assume its standard API contracts.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards** for Node.js security (e.g., latest Express vulnerabilities, TLS standards).
    *   **Validation:** Use `docfork` to verify *every* external API signature (e.g., `npm install` commands, Docker builds).
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code, ensuring SOLID principles are applied to middleware.

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
*   **PRIMARY SCENARIO: WEB / APP / GUI (Node.js Backend)**
    *   **Stack:** **TypeScript (Strict)** is the mandated language standard for all new logic, even if the template initially used pure JS. Migrate configurations to use TypeScript tooling where possible. Core runtime is **Node.js 22 LTS**. Framework: **Express 5.x** (if available, otherwise latest stable 4.x).
    *   **Lint/Test:** **Biome** (for Lint/Format speed) + **Vitest** (Unit/Integration testing framework, favored over Jest for modern speed) + **Playwright** (for E2E if GUI components are added).
    *   **Architecture:** Feature-Sliced Design (FSD) principles adapted for a Monolithic Backend Structure, ensuring clear separation between `routes`, `services`, and `data` layers.

## 4. VERIFICATION COMMANDS
*   **LINT & FORMAT:** `npx @biomejs/biome check --apply .`
*   **TEST (Unit/Integration):** `npx vitest`
*   **SETUP (Standardized):** `npm ci && npm run build`
*   **START (Development):** `npm run dev`

## 5. ARCHITECTURAL PRINCIPLES CHECKLIST
*   [X] **SOLID:** Dependencies injected (where applicable), Single Responsibility observed in service functions.
*   [X] **DRY:** Template reuse prioritized via EJS partials and shared middleware functions.
*   [X] **YAGNI:** Keep dependencies minimal; focus on providing a clean, base structure only.

</details>

## 🚀 Getting Started

### Prerequisites
*   Node.js (v18+ recommended, v20+ preferred)
*   npm or Yarn/pnpm (npm used in scripts)
*   Docker (for containerized deployment)

### Installation & Setup

1.  **Clone Repository (Use Template Feature Recommended):**
    bash
    # RECOMMENDED: Use GitHub Template button above
    # git clone https://github.com/chirag127/Express-Kickstart-NodeJS-Web-App-Template.git my-new-project
    # cd my-new-project
    

2.  **Install Dependencies:**
    bash
    npm ci
    

3.  **Configure Environment:**
    Create a `.env` file in the root directory based on `.env.example`.

### Development Scripts

| Script | Command | Description |
| :--- | :--- | :--- |
| **Start Dev** | `npm run dev` | Runs the server with hot-reloading (via Nodemon/similar setup). |
| **Build** | `npm run build` | Compiles TypeScript/Minifies assets (if applicable to JS template). |
| **Test** | `npm run test` | Executes Biome linting and Vitest unit tests. |
| **Format** | `npm run format` | Applies Biome formatting rules across the codebase. |
| **Start Prod** | `npm start` | Starts the optimized production server. |
| **Containerize** | `docker build -t myapp .` | Builds the production Docker image. |

## 🛡️ Development Principles

This template is built adhering to these core software engineering tenets:

1.  **SOLID:** Focusing on high cohesion and loose coupling.
2.  **DRY:** Eliminating redundant code via reusable modules and shared middleware.
3.  **YAGNI:** Do not build features that are not immediately required by the core template objective.

## 🤝 Contribution Guidelines

Please review the detailed guidelines in [.github/CONTRIBUTING.md](./.github/CONTRIBUTING.md) before submitting pull requests or logging issues.

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the [LICENSE](./LICENSE) file for details.