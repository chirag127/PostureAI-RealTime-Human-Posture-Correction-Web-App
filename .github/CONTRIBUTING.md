# Contributing to PostureGuard-AI-Human-Posture-Analysis-Web-Platform

We welcome contributions to the PostureGuard-AI-Human-Posture-Analysis-Web-Platform! To ensure a high-quality, collaborative, and secure development environment, please adhere to the following guidelines.

## 1. Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [CODE_OF_CONDUCT_EMAIL_OR_LINK].

## 2. Prerequisites

Before contributing, please ensure you have:

*   **Git Installed:** For version control.
*   **Node.js & npm/yarn/pnpm:** The project utilizes modern JavaScript/TypeScript. Check `package.json` for specific version requirements.
*   **Apex Toolchain:** Familiarity with the technologies defined in the `AGENTS.md` file (Biome, Vitest, Playwright, Vite, TypeScript).
*   **Understanding of AI/Computer Vision Concepts:** Basic knowledge of posture analysis, real-time video processing, and AI feedback mechanisms is beneficial.

## 3. Getting Started

1.  **Fork the Repository:** Create your own fork of the `PostureGuard-AI-Human-Posture-Analysis-Web-Platform` repository.
2.  **Clone Your Fork:** Clone your forked repository locally:
    ```bash
    git clone https://github.com/<YOUR_USERNAME>/PostureGuard-AI-Human-Posture-Analysis-Web-Platform.git
    cd PostureGuard-AI-Human-Posture-Analysis-Web-Platform
    ```
3.  **Add Upstream Remote:** Configure your local repository to track the main repository:
    ```bash
    git remote add upstream https://github.com/APEX-AI-ARCHITECTS/PostureGuard-AI-Human-Posture-Analysis-Web-Platform.git
    ```
4.  **Keep Your Fork Synced:** Regularly fetch changes from the upstream and merge them into your local `main` branch:
    ```bash
    git fetch upstream
    git checkout main
    git merge upstream/main
    git push origin main
    ```
5.  **Create a Feature Branch:** For every new feature or bug fix, create a dedicated branch:
    ```bash
    git checkout -b feature/your-feature-name
    # or
    git checkout -b fix/your-bug-description
    ```

## 4. Development Workflow

We follow the **Apex Recursive Perfection Loop** and a strict CI/CD pipeline.

1.  **Code:** Implement your changes on your feature branch.
2.  **Lint & Format:** Automatically format and lint your code. The project uses **Biome** for both. Ensure your code passes these checks *before* committing.
    ```bash
    # Install dependencies (if not already done)
    npm install

    # Run Biome for checking and applying fixes
    npx @biomejs/biome check --apply
    ```
3.  **Test:** Write and run comprehensive unit and integration tests using **Vitest** and end-to-end tests with **Playwright**.
    ```bash
    # Run Vitest tests
    npm run test:unit

    # Run Playwright tests
    npm run test:e2e
    ```
4.  **Commit:** Commit your changes following the **Conventional Commits** specification.
    ```bash
    # Example: feat(posture): Add real-time analysis for side profile
    git commit -m "feat(posture): Add real-time analysis for side profile"
    ```
5.  **Push:** Push your feature branch to your fork.
    ```bash
    git push origin feature/your-feature-name
    ```
6.  **Pull Request:** Open a Pull Request against the `main` branch of the **APEX-AI-ARCHITECTS** repository.

## 5. Pull Request Guidelines

*   **Target Branch:** All pull requests should target the `main` branch.
*   **Clear Description:** Provide a detailed description of your changes, including the problem solved, the solution implemented, and any relevant context.
*   **Link Issues:** Reference any related GitHub issues using keywords like `Closes #123` or `Fixes #456`.
*   **Screenshots/GIFs:** For UI changes, include visual examples.
*   **Tests:** Ensure all tests pass and that new functionality is covered by adequate tests.
*   **Code Reviews:** Be prepared to respond to feedback from reviewers and make necessary adjustments.

## 6. Contribution Areas

We encourage contributions in the following areas:

*   **AI Model Improvements:** Enhancing posture detection accuracy and efficiency.
*   **Real-time Computer Vision:** Optimizing webcam feed processing.
*   **User Interface & Experience:** Improving the usability and aesthetic (Liquid Glass + Neo-Brutalist + Material You 3.0).
*   **Performance Optimization:** Reducing latency and resource consumption.
*   **Testing & Quality Assurance:** Expanding test coverage and identifying edge cases.
*   **Documentation:** Improving clarity and completeness of project documentation.
*   **New Features:** Based on community feedback and the project roadmap.

## 7. Reporting Issues

*   **Search First:** Before reporting a new issue, search existing issues to see if it has already been reported.
*   **Clear Title:** Use a concise and descriptive title.
*   **Detailed Description:** Provide clear steps to reproduce the issue, expected behavior, and actual behavior.
*   **Environment Details:** Include information about your OS, browser, and relevant software versions.
*   **Screenshots/Logs:** Attach relevant screenshots or console logs.

## 8. Architectural Principles & Standards

All contributions must adhere to the project's core principles:

*   **Apex Technical Authority Standards:** As detailed in `AGENTS.md`.
*   **SOLID Principles:** Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion.
*   **DRY & KISS:** Don't Repeat Yourself, Keep It Simple, Stupid.
*   **CQS:** Command-Query Separation.
*   **12-Factor App Principles.**
*   **Zero-Trust Security Model.**
*   **Semantic HTML & Accessibility (WCAG 2.1 AA).**
*   **Performance Optimization (INP < 200ms).**

## 9. Licensing

All contributions are made under the terms of the **CC BY-NC 4.0 License**. By submitting a pull request, you agree to license your contributions under this license.

Thank you for contributing to PostureGuard!
