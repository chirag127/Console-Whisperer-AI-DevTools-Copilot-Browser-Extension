# ConsoleAI-DevTools-Copilot-Browser-Extension

> AI-Powered Copilot for Browser Developer Tools: Real-time Error Analysis, Code Optimization, and Debugging Insights.

<p align="center">
  <img src="https://img.shields.io/badge/STATUS-ACTIVE-brightgreen" alt="Active Project">
  <img src="https://img.shields.io/github/v/tag/chirag127/ConsoleAI-DevTools-Copilot-Browser-Extension?sort=semver" alt="Latest Release">
  <img src="https://img.shields.io/github/license/chirag127/ConsoleAI-DevTools-Copilot-Browser-Extension" alt="License">
  <img src="https://img.shields.io/github/stars/chirag127/ConsoleAI-DevTools-Copilot-Browser-Extension?style=flat-square" alt="GitHub Stars">
</p>

## ✨ Features

*   **Real-time Error Analysis:** Instantly interpret console errors with AI-driven explanations and potential fixes.
*   **Code Optimization Suggestions:** Receive context-aware recommendations to improve performance and efficiency.
*   **Debugging Insights:** Leverage AI to identify root causes of bugs and suggest debugging strategies.
*   **Seamless Integration:** Works directly within your browser's developer tools.
*   **Productivity Boost:** Reduce debugging time and accelerate development cycles.

## 🚀 Tech Stack

*   **Frontend:** JavaScript, HTML, CSS
*   **Browser Extension APIs:** Chrome Extension APIs / WebExtension Polyfill
*   **AI Integration:** LLM (e.g., GPT, Gemini) for analysis and generation.
*   **Development Environment:** Vite (for build tooling if applicable for extensions)

## 🏛️ Architecture

This browser extension follows a modular architecture designed for efficiency and maintainability within the browser's extension environment.

mermaid
graph TD
    A[Browser DevTools Console] --> B(Extension Content Script);
    B --> C(Extension Background Script);
    C --> D{AI Analysis Service};
    D --> C;
    C --> B;
    B --> E[User Interface Overlay];


## 📋 Table of Contents

*   [Features](#-features)
*   [Tech Stack](#-tech-stack)
*   [Architecture](#-architecture)
*   [Getting Started](#-getting-started)
*   [Development](#-development)
*   [Contributing](#-contributing)
*   [License](#-license)
*   [AI Agent Directives](#-ai-agent-directives)

## 🚀 Getting Started

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/ConsoleAI-DevTools-Copilot-Browser-Extension.git
    cd ConsoleAI-DevTools-Copilot-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    # Using npm (standard for many JS projects)
    npm install
    
    *Note: If using a specific package manager like yarn or pnpm, adjust accordingly.* 

3.  **Build the extension:**
    bash
    npm run build
    

4.  **Load the extension in your browser:**
    *   Open your browser's extension management page (e.g., `chrome://extensions/` for Chrome).
    *   Enable "Developer mode".
    *   Click "Load unpacked" and select the `dist` (or equivalent build output) folder from the project.

### Configuration

*   **API Keys:** You may need to configure API keys for the AI service. Refer to the environment variable documentation within the project.

## 🛠️ Development

### Running in Development Mode

To run the extension with live-reloading and debugging capabilities:

bash
npm run dev


This command typically starts a development server and rebuilds the extension upon file changes. Follow the browser loading steps above with the development output folder.

### Scripts

| Script      | Description                                                                 |
| :---------- | :-------------------------------------------------------------------------- |
| `dev`       | Starts the development server with hot-reloading.                           |
| `build`     | Compiles the extension for production deployment.                           |
| `lint`      | Runs the linter to check for code style and potential errors.               |
| `test`      | Executes unit and integration tests.                                        |
| `test:e2e`  | Executes end-to-end tests (if applicable).                                  |

## 🛡️ Security

*   **API Key Management:** Sensitive API keys should **never** be committed directly to the repository. Use environment variables or secure configuration management.
*   **Input Sanitization:** Sanitize all user inputs and data fetched from external sources to prevent XSS and other vulnerabilities.
*   **Dependency Auditing:** Regularly audit dependencies for known vulnerabilities using tools like `npm audit`.

## 🤝 Contributing

Contributions are welcome! Please refer to the [CONTRIBUTING.md](https://github.com/chirag127/ConsoleAI-DevTools-Copilot-Browser-Extension/blob/main/.github/CONTRIBUTING.md) file for detailed guidelines on how to submit bug reports, feature requests, and pull requests.

## 📄 License

This project is licensed under the **CC BY-NC 4.0** license - see the [LICENSE](https://github.com/chirag127/ConsoleAI-DevTools-Copilot-Browser-Extension/blob/main/LICENSE) file for details.

---

<details>
<summary>🤖 AI AGENT DIRECTIVES</summary>

## SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

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

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `ConsoleAI-DevTools-Copilot-Browser-Extension`, is a JavaScript Browser Extension.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript/JavaScript)**
    *   **Stack:** This project leverages **JavaScript** with modern browser extension APIs. Development tooling may include **Vite** for efficient builds and bundling. Frameworks like React or Vue.js might be used for UI components within the extension if necessary, but core functionality relies on pure JavaScript and Extension APIs.
    *   **Linting & Formatting:** **Biome** (for ultra-fast linting and formatting) is the standard. Configuration is managed via `biome.json`.
    *   **Testing:** **Vitest** for fast unit testing and **Playwright** for robust End-to-End (E2E) testing are the mandated tools. Testing strategy focuses on isolating extension components and simulating user interactions.
    *   **Architecture:** Adheres to **Feature-Sliced Design (FSD)** principles where applicable for organizing frontend code, ensuring scalability and maintainability. Extension logic is typically separated into content scripts, background scripts, and popup UIs.
    *   **AI Integration:** Deeply integrated with a chosen LLM API (e.g., OpenAI's GPT series, Google Gemini) for intelligent analysis and code generation. Prioritize secure handling of API keys and efficient data transfer. Models such as `gpt-4-turbo-preview` or equivalent are preferred for advanced reasoning.

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Rust/Go) - *Not applicable for this project.***
*   **TERTIARY SCENARIO C: DATA / AI / SCRIPTS (Python) - *Not applicable for this project.***

### 4. APEX DEVELOPMENT PRINCIPLES
*   **SOLID:** Design software components that are Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion.
*   **DRY:** "Don't Repeat Yourself." Ensure code reusability and avoid redundancy.
*   **YAGNI:** "You Aren't Gonna Need It." Implement features only when required.
*   **KISS:** "Keep It Simple, Stupid." Favor straightforward solutions.

### 5. VERIFICATION COMMANDS
*   **Lint & Format:** `npm run lint` (or `npx @biomejs/biome lint --apply`)
*   **Unit Tests:** `npm test` (or `npx vitest`)
*   **E2E Tests:** `npx playwright test`
*   **Build:** `npm run build`

</details>
