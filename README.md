# PostureGuard-AI-Posture-Correction-Desktop-App

[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App/ci.yml?style=flat-square)](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App/actions/workflows/ci.yml)
[![codecov](https://img.shields.io/codecov/c/github/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App?style=flat-square)](https://codecov.io/github/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App)
[![Tech Stack](https://img.shields.io/badge/TechStack-TS%7CVite%7CTauri%7CTailwindCSS-blue?style=flat-square)]()
[![Lint/Format](https://img.shields.io/badge/Lint%2FFormat-Biome-orange?style=flat-square)]()
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-red?style=flat-square)](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App?style=flat-square)]()

[<img src="https://img.shields.io/github/stars/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App?style=social&label=Star%20this%20Repo"/>](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App)

## BLUF
PostureGuard leverages AI-powered real-time computer vision analysis via your webcam to detect, alert, and guide users toward improved posture, fostering ergonomic health and long-term well-being.

## Architecture Overview

mermaid
graph TD
    A[Webcam Input] --> B(Real-time Pose Estimation)
    B --> C{Posture Analysis Engine}
    C --> D{Feedback & Alerting System}
    D --> E[User Interface (React/Tauri)]
    E --> F(Ergonomic Health Improvement)


## Table of Contents

*   [BLUF](#bluf)
*   [Architecture Overview](#architecture-overview)
*   [AI Agent Directives](#ai-agent-directives)
*   [Development Standards](#development-standards)
*   [Setup](#setup)
*   [Scripts](#scripts)
*   [Contributing](#contributing)
*   [License](#license)

<details>
<summary>🤖 AI Agent Directives (December 2025 Edition)</summary>

## SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the **Apex Toolchain**. This repository, `PostureGuard-AI-Posture-Correction-Desktop-App`, is a Desktop Application.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend - Desktop Variant)**
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native Desktop), TailwindCSS v4.
    *   **Lint/Test:** Biome (Speed & Formatting) + Vitest (Unit Testing) + Playwright (End-to-End Testing).
    *   **Architecture:** Employing **Feature-Sliced Design (FSD)** for modularity and maintainability.
    *   **State Management:** Signals (Standardized).

---

## 4. DEVELOPMENT & TESTING PROTOCOLS
*   **CODE QUALITY:**
    *   **Linting & Formatting:** **Biome** is the mandated tool. Ensure all code adheres to the configured Biome standards.
    *   **Type Safety:** **TypeScript** with `strict: true` enabled in `tsconfig.json` is mandatory.
*   **TESTING STRATEGY:**
    *   **Unit Tests:** Use **Vitest** for comprehensive unit testing. Aim for >80% code coverage.
    *   **Integration Tests:** Covered by Vitest where applicable.
    *   **End-to-End (E2E) Tests:** Utilize **Playwright** for E2E testing, simulating real user interactions within the Tauri application.
    *   **Coverage Reporting:** Integrate with **Codecov** for automated coverage tracking.

---

## 5. RELEASE MANAGEMENT & CI/CD
*   **CI/CD PIPELINE:** Configure GitHub Actions (`ci.yml`) to automate build, lint, test, and release processes.
*   **DEPENDENCY MANAGEMENT:** Utilize **npm/yarn** via Vite's ecosystem. Ensure `package-lock.json` or `yarn.lock` is committed.
*   **NATIVE BUILDS:** Tauri's build process handles native compilation. CI must support creating installers/bundles for target platforms.

---

## 6. SECURITY MANDATES (DECEMBER 2025)
*   **VULNERABILITY SCANNING:** Integrate tools like `npm audit` or `yarn audit` into the CI pipeline. Leverage Dependabot for automated dependency security updates.
*   **SECRET MANAGEMENT:** **NEVER** commit secrets directly. Use environment variables or Tauri's secure process management features.
*   **COMPUTER VISION SAFETY:** Sanitize and validate all inputs to computer vision models. Ensure no sensitive personal data is stored unnecessarily. Be mindful of bias in AI models.
*   **LICENSE COMPLIANCE:** Adhere strictly to the terms of the `CC BY-NC 4.0` license. Ensure all dependencies are compatible.

---

## 7. PROJECT ARCHIVAL PROTOCOL
*   **RETIRING PRODUCTS:** Archived repositories are "Retired Products," not junk. Maintain professional metadata (name, description, topics) and documentation.
*   **LEGACY CODE:** Ensure legacy code remains understandable and maintainable, even when deprecated.

---

</details>

## Development Standards

We adhere to the following principles for building robust and maintainable software:

*   **SOLID:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
*   **DRY:** Don't Repeat Yourself.
*   **YAGNI:** You Ain't Gonna Need It.
*   **KISS:** Keep It Simple, Stupid.
*   **FSD (Feature-Sliced Design):** For modular frontend architecture.

## Setup

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App.git
    cd PostureGuard-AI-Posture-Correction-Desktop-App
    

2.  **Install Dependencies:**
    bash
    # Using npm
    npm install

    # Or using yarn
    # yarn install
    

3.  **Set up Environment Variables (if any):**
    *(Refer to `.env.example` for required variables)*

## Scripts

| Script Name        | Description                                                                |
| :----------------- | :------------------------------------------------------------------------- |
| `npm run dev`      | Starts the development server with hot-reloading.                          |
| `npm run build`    | Builds the production-ready application for Tauri.                         |
| `npm run lint`     | Runs Biome to check and format code.                                       |
| `npm test`         | Executes all unit and integration tests using Vitest.                      |
| `npm run test:e2e` | Runs end-to-end tests using Playwright.                                    |
| `npm run preview`  | Serves the built application locally for preview.                          |

## Contributing

We welcome contributions! Please see the [CONTRIBUTING.md](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App/blob/main/.github/CONTRIBUTING.md) file for detailed guidelines on how to submit pull requests, report bugs, and suggest features.

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the [LICENSE](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Desktop-App/blob/main/LICENSE) file for more details.
