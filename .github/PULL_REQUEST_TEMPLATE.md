```markdown
## Pull Request

Thank you for contributing to Console Whisperer!

Please provide a clear and concise description of your changes.

### PR Checklist:

- [ ] **1. Description of Changes:**
  -   A clear and concise summary of the changes.
  -   Why is this change necessary? What problem does it solve?
  -   Link to any related issues or pull requests.

- [ ] **2. Code Quality & Testing:**
  -   [ ] I have followed the project's code style guidelines.
  -   [ ] My code has no linting errors (run `biome check`).
  -   [ ] My code includes comprehensive unit tests (run `vitest`).
  -   [ ] All tests pass.
  -   [ ] I have considered edge cases and error handling.

- [ ] **3. Documentation:**
  -   [ ] I have updated the documentation (README, etc.) if necessary.
  -   [ ] All new functions/classes are documented.

- [ ] **4. Security:**
  -   [ ] I have considered security implications and followed secure coding practices.
  -   [ ] No sensitive information is included in the commit.

- [ ] **5. Dependencies:**
  -   [ ] If this PR introduces new dependencies, I have listed them in the PR description.
  -   [ ] Dependencies are up-to-date.

### Additional Information:

-   Any specific instructions for reviewers?
-   Screenshots or videos (if applicable).

### Reviewers:

-   Please assign reviewers and/or relevant team members.

---

## AI Agent Directives (For Automated Analysis)

<details>
<summary>Click to Expand</summary>

**Tech Stack:**

*   **Frontend:** TypeScript 6.x, Vite 7, WXT, Signals
*   **Linting:** Biome
*   **Testing:** Vitest (Unit), Playwright (E2E)
*   **Build/Bundling:** Vite

**Architectural Patterns:**

*   Feature-Sliced Design (FSD)
*   SOLID principles (SRP, OCP, LSP, ISP, DIP).
*   CQS (Command Query Separation).

**Verification Commands:**

*   `biome check --apply .` (Format & Lint)
*   `vitest` (Run Unit Tests)
*   `playwright test` (Run E2E Tests)
*   `npm run build` (Build Production)

</details>
