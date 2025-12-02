# PostureGuard-AI-Posture-Correction-Web-App

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/PostureGuard-AI-Posture-Correction-Web-App/ci.yml?label=Build&style=flat-square)](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/PostureGuard-AI-Posture-Correction-Web-App?style=flat-square)](https://codecov.io/gh/chirag127/PostureGuard-AI-Posture-Correction-Web-App)
[![License](https://img.shields.io/github/license/chirag127/PostureGuard-AI-Posture-Correction-Web-App?style=flat-square)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/PostureGuard-AI-Posture-Correction-Web-App?style=flat-square)](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App)

[![Tech Stack](https://img.shields.io/badge/Stack-TypeScript%20%7C%20React%20%7C%20Tauri%20v2-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![Linter/Formatter](https://img.shields.io/badge/Linter-Biome-green?style=flat-square&logo=biome)](https://biomejs.dev/)

[⭐ Star ⭐ this Repo if you find it useful for promoting ergonomic health!]("https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App")

---

PostureGuard is a high-precision, real-time computer vision application that analyzes user posture via webcam input to provide immediate, actionable ergonomic feedback. This repository contains the full source for the cross-platform desktop client built on modern web technologies.

This project represents an elite implementation of **WebAssembly-accelerated Pose Estimation** integrated seamlessly into a Tauri container, ensuring minimal latency and maximum user privacy.

## 📐 Architecture Diagram

ascii
                        +-------------------------+
                        |    User Webcam Input    |
                        +------------+------------+
                                     |
                                     v
                       +--------------------------+
                       |   Tauri Rust Core (Native) |
                       | (Handles HW Access/IPC)  |
                       +------------+------------+
                                     |
                                     v
                       +--------------------------+
                       |  WebGL/WebWorker (WASM)  |
                       | (Pose Estimation Model -  |
                       |   e.g., MediaPipe/TF.js) |
                       +------------+------------+
                                     |
                                     v
                 +----------------------------------+
                 |      Frontend (React/Vite)         |
                 | (State Mgmt, UI Rendering, Data) |
                 +------------------+---------------+   (2. TypeScript Strict)
                                    |               
                                    v               
                           +------------------+       (3. FSD Architecture)
                           |   Ergonomic Feedback   |
                           +------------------+


## 📚 Table of Contents

1.  [Features](#-features)
2.  [Technology Stack (The Apex Toolchain)](#-technology-stack-the-apex-toolchain)
3.  [🤖 AI Agent Directives](#-ai-agent-directives)
4.  [Development Setup](#-development-setup)
5.  [Contribution Guidelines](#-contribution-guidelines)
6.  [License](#-license)

## ✨ Features

*   **Real-Time Pose Tracking:** Utilizes advanced computer vision models to track 30+ key body landmarks instantly.
*   **Ergonomic Scoring:** Generates a composite score based on neck angle, back curvature, and wrist positioning.
*   **Cross-Platform Desktop:** Packaged using Tauri v2, running natively on Windows, macOS, and Linux.
*   **Performance Optimized:** Frontend built with **Vite 7** and utilizes **Web Workers** or **WASM** to offload heavy computation from the main thread.
*   **Strict Typing:** Enforced using **TypeScript** across the entire codebase to eliminate runtime surprises.

## ⚙️ Technology Stack (The Apex Toolchain)

| Category | Technology | Rationale |
| :--- | :--- | :--- |
| **Core Framework** | React (v19+) | Component-based UI architecture. |
| **Bundling** | Vite 7 | Sub-millisecond HMR and rapid build times. |
| **Desktop Runtime** | Tauri v2 | Modern, secure, and small binary footprint. |
| **Language** | TypeScript (Strict Mode) | Enforcing 100% type safety. |
| **Styling** | TailwindCSS v4 | Utility-first, highly maintainable styling. |
| **Linting/Formatting** | Biome | Unifying linting, formatting, and static analysis speed. |
| **Testing** | Vitest (Unit) / Playwright (E2E) | Comprehensive verification strategy. |
| **Architecture** | Feature-Sliced Design (FSD) | Ensuring scalable and decoupled application layers. |

## 🤖 AI Agent Directives

<details>
<summary><strong>Apex Architectural Alignment & Verification Commands</strong></summary>

### **A. Core Principles & Architecture Mandate**

1.  **SOLID Compliance:** All application services (e.g., `PostureService`, `DataPersistor`) must rigorously adhere to the **Single Responsibility Principle (SRP)**. Dependency Injection patterns are mandatory for complex components.
2.  **DRY Enforcement:** Abstract common UI patterns (e.g., ScoreDisplay) into reusable FSD *shared* layers.
3.  **YAGNI Protocol:** Only implement features explicitly required by the current roadmap. Avoid premature abstraction in the computational pipeline.
4.  **FSD Structure:** Strict adherence to the Feature-Sliced Design pattern:
    *   `app/` (App initialization, layout)
    *   `processes/` (High-level user flows)
    *   `pages/` (Routing targets)
    *   `widgets/` (Reusable UI components tied to specific features)
    *   `features/` (Business logic implementations)
    *   `entities/` (Data models and core domain objects)
    *   `shared/` (Primitives, generic utilities, UI elements).

### **B. Technology Stack & Verification**

*   **Language Standard:** TypeScript 6.x targeting ES2022+. Strict mode is enabled in `tsconfig.json`.
*   **Linter/Formatter:** **Biome** is the sole arbiter of code style. All commits must pass `biome check --apply`.
*   **Testing Strategy:**
    *   **Unit Tests (`*.test.ts`):** Cover all `entities/` and `shared/` logic using **Vitest**.
    *   **Integration/E2E Tests:** Cover the complete user journey (webcam access request -> posture analysis -> feedback display) using **Playwright**.

### **C. Self-Correction and Future-Proofing**

*   **Dependency Management:** Use `npm` and lock files must be committed. Future upgrades (e.g., Tauri v3, React 20) should be managed via the `scripts/upgrade.sh` (hypothetical) or by performing a clean audit via `npm outdated` followed by manual review.
*   **Performance Goal:** Latency from frame capture to UI update must remain under 100ms on modern hardware.

</details>

## 🚀 Development Setup

This repository uses **TypeScript**, **Vite**, and **Tauri**. Ensure Node.js (v20+) and Rust toolchain are installed.

### Prerequisites

1.  **Node.js & npm/pnpm/uv:** Install Node.js LTS (or higher).
2.  **Rust Toolchain:** Install via `rustup`.

### Installation Steps

bash
# 1. Clone the repository
git clone https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App.git
cd PostureGuard-AI-Posture-Correction-Web-App

# 2. Install Dependencies (Using npm for web stack simplicity)
npm install

# 3. (Tauri Requirement) Ensure Rust dependencies are built
npm run tauri:build  # Or just run dev first


### Available Scripts

| Command | Description | Apex Standard |
| :--- | :--- | :--- |
| `npm run dev` | Starts the development server with HMR (Vite). | High-Velocity Development |
| `npm run tauri:dev` | Builds and runs the Tauri desktop application. | Native Environment Test |
| `npm run build` | Creates optimized production builds for Web/Tauri. | Zero-Defect Release Candidate |
| `npm run lint` | Runs Biome check across TypeScript and CSS files. | Static Analysis Enforcement |
| `npm run test:unit` | Runs Vitest unit tests. | Logic Integrity Verification |
| `npm run test:e2e` | Runs Playwright end-to-end scenarios. | User Journey Validation |

## 🤝 Contribution Guidelines

Contributions are welcome following the **Zero-Defect, High-Velocity** mandate. Please review the dedicated `.github/CONTRIBUTING.md` file for detailed procedures on commit etiquette, PR templates, and branch naming conventions.

All contributions must pass CI checks defined in `.github/workflows/ci.yml`.

## 🛡️ Security

Security is paramount, especially when handling webcam input locally. Refer to `.github/SECURITY.md` for reporting vulnerabilities. This application strictly adheres to local-only processing principles; **no raw video data leaves the user's machine**.

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the `LICENSE` file for full details.
