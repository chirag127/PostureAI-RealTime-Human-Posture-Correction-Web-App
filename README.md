# PostureGuard-AI-Posture-Correction-Web-App

<!-- Hero Banner/Logo Placeholder -->
<p align="center">
  <img src="https://raw.githubusercontent.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App/main/.github/assets/logo.png" alt="PostureGuard Logo" width="250"/>
</p>

<p align="center">
  <a href="https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App/actions/workflows/ci.yml" target="_blank">
    <img src="https://img.shields.io/github/actions/workflow/status/chirag127/PostureGuard-AI-Posture-Correction-Web-App/ci.yml?branch=main&style=flat-square&label=Build%20Status" alt="Build Status">
  </a>
  <a href="https://codecov.io/gh/chirag127/PostureGuard-AI-Posture-Correction-Web-App" target="_blank">
    <img src="https://img.shields.io/codecov/c/github/chirag127/PostureGuard-AI-Posture-Correction-Web-App?style=flat-square&token=YOUR_CODECOV_TOKEN" alt="Code Coverage">
  </a>
  <img src="https://img.shields.io/badge/Tech%20Stack-React%20%7C%20Vite%20%7C%20Tauri%20%7C%20TS-blueviolet?style=flat-square" alt="Tech Stack">
  <img src="https://img.shields.io/badge/Lint%2FFormat-Biome-informational?style=flat-square" alt="Lint/Format">
  <a href="https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App/blob/main/LICENSE" target="_blank">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg?style=flat-square" alt="License">
  </a>
  <a href="https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App/stargazers" target="_blank">
    <img src="https://img.shields.io/github/stars/chirag127/PostureGuard-AI-Posture-Correction-Web-App?style=flat-square&color=yellow" alt="GitHub Stars">
  </a>
</p>

<p align="center">
  Star ⭐ this Repo!
</p>

## Bluf (Bottom Line Up Front)

PostureGuard is an advanced AI-powered desktop application that leverages real-time computer vision via your webcam to meticulously analyze and correct your posture. By providing instant, actionable feedback, it proactively promotes ergonomic health, prevents musculoskeletal strain, and enhances overall well-being during prolonged computer use.

## 🚀 Key Features

*   **Real-time AI Posture Analysis:** Utilizes cutting-edge pose estimation models to detect and track key anatomical points.
*   **Instant Feedback System:** Delivers immediate visual and auditory cues for posture correction.
*   **Customizable Ergonomic Alerts:** Configure personalized reminders and thresholds for ideal posture.
*   **Privacy-First Design:** All processing occurs locally on your device; no video data is sent to the cloud.
*   **Cross-Platform Compatibility:** Built with Tauri for a lightweight, native desktop experience across Windows, macOS, and Linux.

## 🧠 Architecture Overview: Feature-Sliced Design (FSD)

PostureGuard is structured using the Feature-Sliced Design (FSD) methodology, ensuring a highly scalable, maintainable, and testable codebase. This layered approach promotes strict module boundaries and clear dependencies, making feature development and integration seamless.


PostureGuard-AI-Posture-Correction-Web-App/
├── .github/
├── .cargo/         # Tauri/Rust specific configuration
├── src/
│   ├── app/        # Global logic, routing, layout
│   │   ├── providers/ # Context providers, global state
│   │   └── index.tsx  # Main entry point
│   ├── entities/   # Core domain logic, e.g., PostureDetection, UserPreferences
│   │   ├── posture-model/
│   │   ├── user-settings/
│   │   └── ...
│   ├── features/   # Specific user-facing functionalities, e.g., RealtimeFeedback, PostureReport
│   │   ├── real-time-feedback/
│   │   ├── settings-management/
│   │   └── ...
│   ├── pages/      # Full-page components, composed of features/widgets
│   │   ├── main/
│   │   ├── settings/
│   │   └── ...
│   ├── shared/     # Reusable UI components, utilities, types, API clients
│   │   ├── ui/
│   │   ├── lib/
│   │   ├── api/
│   │   └── ...
│   ├── widgets/    # Combinations of entities and features, e.g., PostureDisplay, FeedbackIndicator
│   │   ├── posture-visualizer/
│   │   ├── alert-system/
│   │   └── ...
│   └── main.ts     # Tauri entry point, Rust backend logic
├── public/
├── index.html
├── package.json
├── Cargo.toml      # Tauri/Rust build configuration
├── vite.config.ts
├── tailwind.config.ts
├── tsconfig.json
└── ...


## 📋 Table of Contents

*   [Bluf (Bottom Line Up Front)](#bluf-bottom-line-up-front)
*   [🚀 Key Features](#-key-features)
*   [🧠 Architecture Overview: Feature-Sliced Design (FSD)](#-architecture-overview-feature-sliced-design-fsd)
*   [📋 Table of Contents](#-table-of-contents)
*   [🤖 AI Agent Directives](#-ai-agent-directives)
*   [🛠️ Development Setup](#️-development-setup)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
    *   [Scripts](#scripts)
*   [🏛️ Core Principles](#️-core-principles)
*   [🤝 Contributing](#-contributing)
*   [📄 License](#-license)

## 🤖 AI Agent Directives

<details>
<summary>⚡️ **CLICK TO EXPAND: APEX AI AGENT DIRECTIVES (DECEMBER 2025 EDITION)** ⚡️</summary>
<br>

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

### 2. INPUT PROCESSING & COGNITION
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

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `PostureGuard-AI-Posture-Correction-Web-App`, is a desktop application primarily built with TypeScript, React, and Tauri for the frontend, with Rust for the native backend.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend & Native Backend)**
    *   **Stack:** This project leverages **TypeScript (Strict Mode)**, **React 19+** (with Signals for state management), **Vite 7+** (using Rolldown), **TailwindCSS v4** (for utility-first styling), and **Tauri v2+** for cross-platform native application development. The native backend logic is implemented in **Rust**.
    *   **Lint/Test:** **Biome** (for ultra-fast linting, formatting, and type-aware checks), **Vitest** (for lightning-fast unit and component testing), and **Playwright** (for robust end-to-end testing of the Tauri application UI).
    *   **Architecture:** Adheres strictly to **Feature-Sliced Design (FSD)** principles, promoting high cohesion, low coupling, and clear separation of concerns across layers (app, pages, features, widgets, entities, shared).
    *   **AI Integration:** Real-time computer vision and pose estimation capabilities are primarily handled through optimized Rust-based libraries (e.g., OpenCV wrappers, custom inference engines) exposed via Tauri's IPC, ensuring high performance and local data processing for privacy.

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Rust) - *Applicable for the Tauri backend.***
    *   **Stack:** Rust (Cargo) for high-performance, memory-safe native backend components.
    *   **Lint:** `cargo clippy` for comprehensive linting.
    *   **Architecture:** Hexagonal Architecture (Ports & Adapters) or a layered approach within the Rust backend to clearly separate domain logic from infrastructure concerns (e.g., webcam access, AI model inference).

---

### 4. ARCHITECTURAL PATTERNS & PRINCIPLES
*   **SOLID Principles:** Strictly applied for maintainable and scalable code (Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion).
*   **DRY (Don't Repeat Yourself):** Eliminate redundant code; abstract common functionalities.
*   **YAGNI (You Ain't Gonna Need It):** Build only what is necessary for current requirements; avoid speculative over-engineering.
*   **Test-Driven Development (TDD):** Adopt TDD for new feature development and bug fixes, ensuring comprehensive test coverage.
*   **Immutable State:** Favor immutable data structures and pure functions where possible, especially within React components and state management.
*   **API-First Design:** Treat internal and external interfaces as first-class citizens, designing clear contracts.

---

### 5. VERIFICATION & COMMANDS
*   **SETUP:** `npm install` (frontend), `cargo install` (backend dependencies if needed).
*   **BUILD:** `npm run build` (Tauri bundles frontend and Rust).
*   **RUN (DEV):** `npm run dev` (Starts Vite dev server and Tauri dev app).
*   **TEST (UNIT/COMPONENT):** `npm run test` (Vitest).
*   **TEST (E2E):** `npm run test:e2e` (Playwright).
*   **LINT/FORMAT:** `npm run lint`, `npm run format`.
*   **RUST LINT:** `cargo clippy`.
*   **TYPE CHECK:** `npm run typecheck`.

---

### 6. DEVOPS & CI/CD
*   **GitHub Actions:** Mandatory for CI/CD, including automated builds, tests, linting, and release workflows.
*   **Semantic Release:** For automated versioning and release management based on conventional commits.
*   **Containerization (Future):** Explore Docker/Podman for build environments, but Tauri's native bundling is primary.

</details>

## 🛠️ Development Setup

Follow these steps to get PostureGuard up and running on your local machine.

### Prerequisites

Before you begin, ensure you have the following installed:

*   **Node.js** (LTS version, e.g., 20.x) & **npm** (or `pnpm`/`yarn`)
*   **Rust** (Install via `rustup`: `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`)
*   **Tauri Prerequisites** for your specific OS (refer to [Tauri Documentation](https://tauri.app/v1/guides/getting-started/prerequisites/))

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App.git
    cd PostureGuard-AI-Posture-Correction-Web-App
    

2.  **Install Frontend Dependencies:**
    bash
    npm install
    

3.  **Run in Development Mode:**
    This command starts the Vite development server and launches the Tauri application, automatically recompiling Rust changes.
    bash
    npm run dev
    

4.  **Build for Production:**
    bash
    npm run build
    
    The compiled executable will be located in `src-tauri/target/release/`.

### Scripts

The project uses a variety of `npm` scripts for common development tasks:

| Script          | Description                                                    |
| :-------------- | :------------------------------------------------------------- |
| `npm run dev`   | Starts the Vite frontend dev server and the Tauri application. |
| `npm run build` | Builds the Tauri application for production.                   |
| `npm run test`  | Runs unit and component tests with Vitest.                     |
| `npm run test:e2e` | Runs end-to-end tests with Playwright.                       |
| `npm run lint`  | Lints TypeScript and Rust code using Biome and Clippy.         |
| `npm run format`| Formats TypeScript and Rust code using Biome.                  |
| `npm run typecheck` | Performs TypeScript type checking.                         |

## 🏛️ Core Principles

PostureGuard is developed with a strong adherence to modern software engineering principles:

*   **User-Centric Design:** Prioritizing intuitive UI/UX and privacy.
*   **Performance First:** Optimizing AI models and application responsiveness.
*   **Security & Privacy:** Local processing of sensitive webcam data; no cloud uploads.
*   **Maintainability:** Clean, modular, and well-documented code following FSD.
*   **Extensibility:** Designed for easy integration of new features or AI models.

## 🤝 Contributing

We welcome contributions from the community! Please refer to our [Contributing Guidelines](.github/CONTRIBUTING.md) for details on how to get started, report bugs, or suggest enhancements.

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the [LICENSE](LICENSE) file for details.

---