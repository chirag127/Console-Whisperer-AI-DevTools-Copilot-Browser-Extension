# Console-Whisperer-AI-DevTools-Copilot-Browser-Extension

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension/ci.yml?style=flat-square)](https://github.com/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension?style=flat-square)](https://codecov.io/gh/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension)
[![Tech Stack](https://img.shields.io/badge/Tech%20Stack-TypeScript%2C%20Vite%2C%20TailwindCSS%2C%20Tauri-blue?style=flat-square)](https://github.com/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension)
[![Lint/Format](https://img.shields.io/badge/Lint%2FFormat-Biome-brightgreen?style=flat-square)](https://biome.dev/)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square)](https://github.com/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension?style=flat-square)](https://github.com/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension)

**Console-Whisperer** is an intelligent AI copilot designed to augment browser Developer Tools, providing real-time error analysis, code optimization suggestions, and debugging insights directly within your console. It aims to dramatically enhance developer productivity through AI-powered assistance.

## Project Overview

This project aims to be the ultimate AI companion for front-end developers, seamlessly integrating into their existing browser DevTools workflow. It analyzes console logs, network requests, and DOM state to offer actionable insights.

## Architecture

ascii
.
└── Console-Whisperer-AI-DevTools-Copilot-Browser-Extension
    ├── src/
    │   ├── core/
    │   │   ├── ai/
    │   │   ├── analysis/
    │   │   └── services/
    │   ├── ui/
    │   │   ├── components/
    │   │   └── styles/
    │   ├── background/
    │   ├── content/
    │   └── popup/
    ├── vite.config.ts
    ├── tsconfig.json
    ├── biome.json
    ├── package.json
    └── README.md


## Table of Contents

*   [Project Overview](#project-overview)
*   [Architecture](#architecture)
*   [Table of Contents](#table-of-contents)
*   [AI Agent Directives](#ai-agent-directives)
*   [Development Standards](#development-standards)
    *   [Setup](#setup)
    *   [Scripts](#scripts)
    *   [Principles](#principles)
*   [License](#license)
*   [Contributing](#contributing)

## AI Agent Directives

<details>
<summary>Show AI Agent Directives</summary>

This section outlines the core directives and technical specifications for AI agents interacting with this repository. It ensures alignment and consistency in development and operation.

### 1. Identity & Prime Directive

*   **Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
*   **Context:** Current Date is **December 2025**. You are building for the 2026 standard.
*   **Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
*   **Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. Input Processing & Cognition

*   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context. The `README.md` serves as the **Single Source of Truth (SSOT)**.
*   **Research & Validation:** Use `linkup`/`brave` for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**. Use `docfork` to verify *every* external API signature. Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. Context-Aware Apex Tech Stacks (Late 2025 Standards)

*   **PROJECT TYPE:** Web Extension / GUI Application
*   **PRIMARY STACK (LATE 2025):
    *   **Language:** TypeScript 6.x (Strict Mode Enforced)
    *   **Build Tool:** Vite 7 (with Rolldown optimizations)
    *   **Native Integration:** Tauri v2.x
    *   **Extension Framework:** WXT (Web Extension Toolkit)
    *   **State Management:** Signals (Standardized)
    *   **Styling:** TailwindCSS v4
    *   **Linting/Formatting:** Biome (Performance-focused)
    *   **Testing:** Vitest (Unit/Integration), Playwright (E2E)
*   **ARCHITECTURE:** Feature-Sliced Design (FSD) is the mandated pattern for organizing the codebase, promoting modularity and scalability.

### 4. Core Functionality & Compliance

*   **DevTools Integration:** Must seamlessly interface with Chrome/Firefox Developer Tools console API.
*   **AI Model Interaction:** Utilize secure, versioned APIs for AI model communication (e.g., OpenAI GPT-4 Turbo, Anthropic Claude 3 Opus). Prioritize low-latency responses and robust error handling.
*   **Security:** Adhere to OWASP Top 10 for Browser Extensions. Implement Content Security Policy (CSP), sanitize all inputs, and protect against common vulnerabilities.
*   **Performance:** Optimize for minimal memory footprint and CPU usage, especially within the browser extension context.

### 5. Verification Commands

*   **Setup:** `git clone https://github.com/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension.git && cd Console-Whisperer-AI-DevTools-Copilot-Browser-Extension && uv sync`
*   **Lint & Format:** `biome check --apply`
*   **Unit Tests:** `vitest run`
*   **E2E Tests:** `npx playwright test`
*   **Build:** `wxt build --type chrome`

</details>

## Development Standards

### Setup

Follow these steps to set up the development environment:

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/Console-Whisperer-AI-DevTools-Copilot-Browser-Extension.git
    
2.  **Navigate to the project directory:**
    bash
    cd Console-Whisperer-AI-DevTools-Copilot-Browser-Extension
    
3.  **Install dependencies using uv:**
    bash
    uv sync
    

### Scripts

| Script        | Description                                                     |
| :------------ | :-------------------------------------------------------------- |
| `dev`         | Starts the development server with hot-reloading.               |
| `build`       | Builds the production-ready browser extension.                  |
| `lint`        | Runs Biome to check code style and formatting.                  |
| `format`      | Applies Biome formatting to the codebase.                       |
| `test:unit`   | Executes unit and integration tests using Vitest.               |
| `test:e2e`    | Runs end-to-end tests using Playwright.                         |
| `preview`     | Locally previews the production build.                          |

### Principles

*   **SOLID:** Apply principles of Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion.
*   **DRY:** Don't Repeat Yourself. Abstract common logic into reusable functions and components.
*   **YAGNI:** You Aren't Gonna Need It. Avoid implementing features until they are explicitly required.

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the [LICENSE](LICENSE) file for more details.

## Contributing

Contributions are welcome! Please refer to the [CONTRIBUTING.md](.github/CONTRIBUTING.md) file for guidelines on how to submit pull requests and report issues.
