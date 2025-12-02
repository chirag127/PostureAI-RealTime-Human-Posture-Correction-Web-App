---
name: Bug Report
about: Report a bug or unexpected behavior in the application.
title: "Bug: [Describe the issue concisely]"
labels: bug
assignees: "chirag127"

body:
  - type: markdown
    attributes:
      value: | # This is a template for reporting bugs.
        Please provide a clear and detailed description of the bug.
        
        **Repository:** `PostureGuard-AI-Posture-Correction-Web-App`
        **Link:** [https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App](https://github.com/chirag127/PostureGuard-AI-Posture-Correction-Web-App)

        --- # Please ensure all sections below are filled out completely.

  - type: input
    id: reproducible
    attributes:
      label: Steps to Reproduce
      description: Provide a step-by-step guide to reproduce the behavior.
      placeholder: "1. Open the app\n2. Navigate to ...\n3. Click on ..."
    validations:
      required: true

  - type: input
    id: expected_behavior
    attributes:
      label: Expected Behavior
      description: What did you expect to happen?
      placeholder: "The posture analysis should update in real-time."
    validations:
      required: true

  - type: input
    id: actual_behavior
    attributes:
      label: Actual Behavior
      description: What actually happened?
      placeholder: "The posture analysis froze after the first frame."
    validations:
      required: true

  - type: textarea
    id: environment
    attributes:
      label: Environment Details
      description: | # Information about your environment.
        * **OS:** (e.g., Windows 11, macOS Sonoma, Ubuntu 22.04)
        * **Browser:** (e.g., Chrome 120, Firefox 118, Safari 17)
        * **Tauri Version (if applicable):** (e.g., v2.x.x)
        * **React Version (if applicable):** (e.g., v18.x.x)
        * **Node.js Version:** (e.g., v20.x.x)
        * **npm/Yarn Version (if applicable):** (e.g., npm 10.x.x)
        * **Screen Resolution:** (e.g., 1920x1080)
        * **Webcam Model (if known):**
      placeholder: "OS: Windows 11\nBrowser: Chrome 120\nNode.js: v20.10.0"
    validations:
      required: true

  - type: textarea
    id: additional_context
    attributes:
      label: Additional Context
      description: | # Add any other context about the problem here.
        Screenshots, logs, or videos can be very helpful.
        
        **Logs:**
        
        [Paste relevant logs here]
        
        
        **Screenshots/Recordings:**
        [Link to screenshots or recordings if available]
        
        **Relevant Architecture/Code Snippets:**
        [If you can point to specific code that might be related]
      placeholder: "Include any relevant information that might help the maintainers diagnose the issue."
    validations:
      required: false

  - type: textarea
    id: system_info
    attributes:
      label: System Information (AI Agent Directives)
      description: | # Information for AI Agent directives for debugging.
        This section is for AI agents to understand the system context for debugging.
        * **Tech Stack:** TypeScript, Vite, Tauri, React, Biome, (Potential AI Models: Pose Estimation Libraries)
        * **Architecture:** Feature-Sliced Design (FSD) for frontend, Native integration via Tauri.
        * **Core Problem Domain:** Real-time computer vision for posture analysis.
        * **Specific Components:** Webcam access, frame processing, pose estimation algorithms, UI feedback.
      placeholder: "AI agents will use this to identify potential areas of failure."
    validations:
      required: true

  - type: checkboxes
    id: data_privacy
    attributes:
      label: Data Privacy
      description: Confirm that no Personally Identifiable Information (PII) or sensitive data is being shared in this bug report unless absolutely necessary and anonymized.
      options:
        - label: I confirm that this bug report does not contain sensitive PII or unnecessary sensitive data.
          required: true
