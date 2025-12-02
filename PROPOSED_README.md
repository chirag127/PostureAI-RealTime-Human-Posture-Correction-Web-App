# PostureGuard-AI-Posture-Correction-Web-App

An AI-powered web application that leverages real-time computer vision via webcam to analyze and correct human posture, promoting ergonomic health and well-being. Built with React, Vite, and Tauri.

---

## 🤖 AI AGENT DIRECTIVES

<details>
<summary>Click to Expand Agent Directives</summary>

This repository is managed by the **Apex Technical Authority** using the **December 2025 Edition** of the AI Agent Directives.

### 1. Identity & Prime Directive
**Role:** Senior Principal Software Architect and Master Technical Copywriter with 40+ years of elite industry experience. Operating with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is December 2025. Building for the 2026 standard.
**Output Standard:** EXECUTION-ONLY results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. Input Processing & Cognition
*   **Speech-to-Text Interpretation Protocol:** Semantic Correction is **STRICTLY FORBIDDEN** from executing literal typos. Infer technical intent based on project context. `README.md` is the Single Source of Truth (SSOT).
*   **Mandatory MCP Instrumentation:** No Guessing. Use `linkup`/`brave` for December 2025 Industry Standards, Security Threats, and 2026 UI Trends. Use `docfork` to verify *every* external API signature. Engage `clear-thought-two` for architecting complex flows.

### 3. Context-Aware Apex Tech Stacks (Late 2025 Standards)
This project, `PostureGuard-AI-Posture-Correction-Web-App`, is a TypeScript/JavaScript-based Web Application.

*   **PRIMARY SCENARIO: WEB / APP / GUI (Modern Frontend / Desktop App)**
    *   **Stack:** Leverages **TypeScript 6.x (Strict)**, **Vite 7 (Rolldown)** for rapid development, and **Tauri v2.x** for building cross-platform desktop applications from web technologies.
    *   **UI Framework:** **React 19+** with **TailwindCSS v4** for utility-first styling.
    *   **State Management:** Standardized using **Signals (December 2025 Standard)**.
    *   **Linting & Formatting:** **Biome** for ultra-fast code quality checks.
    *   **Testing:** **Vitest** for unit and integration tests, **Playwright** for end-to-end (E2E) testing.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)** principles for maintainable and scalable frontend architecture.
    *   **AI Integration:** Utilizes **OpenCV.js** or similar client-side computer vision libraries for real-time pose estimation. Interacts with backend APIs for advanced AI processing if required, prioritizing secure and efficient data transfer.

### 4. Verification & Execution Commands
*   **Code Quality:** `biome check --apply`
*   **Formatting:** `biome format --write`
*   **Unit Tests:** `npm run test:unit` (or `yarn test:unit`)
*   **E2E Tests:** `npm run test:e2e` (or `yarn test:e2e`)
*   **Build for Production:** `npm run build` (or `yarn build`)
*   **Run Development Server:** `npm run dev` (or `yarn dev`)
*   **Build Desktop App:** `npm run tauri:build` (or `yarn tauri:build`)

### 5. Architectural Principles
*   **SOLID:** Adherence to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion principles.
*   **DRY:** Don't Repeat Yourself – abstract common logic into reusable components and functions.
*   **YAGNI:** You Ain't Gonna Need It – focus on current requirements, avoid speculative feature development.
*   **FSD:** Structure code by features, layers, and segments for clarity and maintainability.

</details>

---

## 🚀 Project Overview

**PostureGuard** is an innovative AI-powered web application designed to promote better posture and ergonomic health. By utilizing your webcam and advanced computer vision algorithms, PostureGuard analyzes your body's pose in real-time, provides immediate feedback, and offers actionable guidance to correct poor posture habits. This fosters a healthier and more productive environment, whether you're working from home or in the office.

---

## ✨ Core Features

*   **Real-time Posture Analysis:** Live webcam feed processed by AI to detect and track body posture.
*   **AI-Powered Correction Guidance:** Intelligent feedback and suggestions to adjust your posture.
*   **Ergonomic Health Focus:** Promotes long-term well-being and reduces strain.
*   **Cross-Platform Desktop App:** Packaged as a native desktop application using Tauri.
*   **Intuitive User Interface:** Built with React and styled with TailwindCSS for a seamless user experience.

---

## 🛠️ Tech Stack

*   **Language:** TypeScript
*   **Bundler/Dev Server:** Vite 7
*   **Frontend Framework:** React 19+
*   **Styling:** TailwindCSS v4
*   **Desktop Packaging:** Tauri v2.x
*   **AI/Computer Vision:** OpenCV.js (Client-Side)
*   **Linting/Formatting:** Biome
*   **Testing:** Vitest (Unit/Integration), Playwright (E2E)
*   **Architecture:** Feature-Sliced Design (FSD)

---

## 📋 Table of Contents

*   [🚀 Project Overview](#-project-overview)
*   [✨ Core Features](#-core-features)
*   [🛠️ Tech Stack](#-tech-stack)
*   [📋 Table of Contents](#-table-of-contents)
*   [🤖 AI Agent Directives](#-ai-agent-directives)
*   [⭐ Contributing](#-contributing)
*   [📜 License](#-license)
*   [🚀 Getting Started](#-getting-started)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
    *   [Running the Development Server](#running-the-development-server)
    *   [Building the Desktop App](#building-the-desktop-app)
*   [📝 Development Scripts](#-development-scripts)
*   [🛡️ Security](#-security)
*   [🌟 Social Proof](#-social-proof)

---

## ⭐ Contributing

Contributions are welcome! Please follow these steps:

1.  **Fork the repository** on GitHub.
2.  **Clone your forked repository** locally: `git clone https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App.git`
3.  **Create a new branch** for your feature or bug fix: `git checkout -b feature/your-feature-name`
4.  **Make your changes** and ensure they adhere to the project's coding standards.
5.  **Test your changes** thoroughly.
6.  **Commit your changes** with clear and concise messages.
7.  **Push your branch** to your fork: `git push origin feature/your-feature-name`
8.  **Open a Pull Request** to the `main` branch of the `chirag127/PostureGuard-AI-Posture-Correction-Web-App` repository.

For more details, please see the [CONTRIBUTING.md](./.github/CONTRIBUTING.md) file.

---

## 📜 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. See the [LICENSE](./LICENSE) file for more details.

---

## 🚀 Getting Started

### Prerequisites

*   **Node.js:** Version 20.x or higher (recommended).
*   **npm** or **yarn** package manager.
*   **Tauri CLI:** Install globally if you plan to build the desktop application: `npm install -g @tauri-apps/cli`
*   **Webcam:** A functional webcam connected to your system.

### Installation

1.  Clone the repository:
    bash
    git clone https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App.git
    cd PostureGuard-AI-Posture-Correction-Web-App
    

2.  Install dependencies:
    bash
    npm install
    # or
    yarn install
    

### Running the Development Server

To start the development server with hot-reloading:

bash
npm run dev
# or
yarn dev


This will typically start the application at `http://localhost:5173` (or a similar port).

### Building the Desktop App

To build a production-ready desktop application for your platform:

bash
npm run tauri:build
# or
yarn tauri:build


This command will bundle your web application and create native executables for Windows, macOS, and Linux.

---

## 📝 Development Scripts

| Script         | Description                                            |
| -------------- | ------------------------------------------------------ |
| `dev`          | Run the development server (Vite + React)              |
| `build`        | Build the web application for production               |
| `lint`         | Run Biome linter                                       |
| `lint:fix`     | Fix linting issues with Biome                          |
| `format`       | Run Biome formatter                                    |
| `format:fix`   | Fix formatting issues with Biome                       |
| `test:unit`    | Run Vitest unit and integration tests                  |
| `test:e2e`     | Run Playwright end-to-end tests                        |
| `tauri:dev`    | Run the Tauri development server (with native features) |
| `tauri:build`  | Build the Tauri desktop application                    |
| `tauri:check`  | Check Tauri dependencies and configuration             |

---

## 🛡️ Security

For security guidelines and best practices, please refer to the [SECURITY.md](./.github/SECURITY.md) file.

---

## 🌟 Social Proof

If you find this project useful, please consider giving it a star ⭐ on GitHub!
