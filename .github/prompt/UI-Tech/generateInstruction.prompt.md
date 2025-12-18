You are acting as a documentation generator for a UI-focused repository.

Your task is to execute the following steps **strictly in order**.  
Each step depends on the output of the previous one.  
Do NOT skip steps. Do NOT merge steps.  
Only proceed to the next step after completing the current one.

All outputs must be written in Markdown and optimized for clarity and reuse.
Assume this repository is a UI project (React, Angular, JS/TS, CSS).

---

## Step 1 — Tech Stack Analysis

Analyze the repository structure and configuration files.

Identify:

- UI frameworks and libraries (React, Angular, etc.)
- Languages used (JS, TS)
- Styling approach (CSS, SCSS, Modules, etc.)
- Build tools
- Linting tools
- Testing tools (or explicitly state if none exist)

Output:

- High-level purpose of the project
- No opinions or recommendations
- Suitable for long-term reference
- Folder structure patterns

Write the output to:
`docs/copilot/tech-stack.md`

Do not proceed to Step 2 until this file content is complete.

---

## Step 2 — Coding Standards

Using:

- The generated `docs/copilot/tech-stack.md`
- The actual patterns observed in the repository

Generate detailed coding standards covering:

- Naming conventions
- Formatting rules
- Component and folder structure
- State management patterns
- Typing conventions (or lack thereof)
- CSS standards and methodology
- Testing conventions (explicitly note if not implemented)

Guidelines:

- Be specific to THIS repository
- Avoid generic best practices unless already reflected in code
- Write for developers and AI tools

Write the output to:
`docs/copilot/coding-standards.md`

Do not proceed to Step 3 until this file content is complete.

---

## Step 3 — Build, Test, and Lint Commands

Scan the repository for:

- npm/yarn scripts
- Build commands
- Lint commands
- Test commands (or explicitly note absence)
- CI/CD configuration (if present)

Include:

- Command examples
- Common flags
- Expected outcomes
- Troubleshooting notes where helpful

Write the output to:
`docs/copilot/build-test.md`

Do not proceed to Step 4 until this file content is complete.

---

## Step 4 — Copilot Instruction File

Using ONLY summaries and references (not full details), generate:

`.github/copilot-instructions.md`

Requirements:

- One-sentence project summary
- Links to:
  - docs/copilot/tech-stack.md
  - docs/copilot/coding-standards.md
  - docs/copilot/build-test.md
- High-level behavioral guidelines for Copilot
- No deep implementation details
- No duplication of content from referenced docs
- Keep total length under 4000 characters

Use phrasing like:
“See docs/copilot/tech-stack.md for full details.”

This file should act as a **thin behavioral contract**, not documentation.

---

## Final Check

Before finishing:

- Ensure there are no contradictions across documents
- Prefer existing patterns over hypothetical improvements
- Ensure instruction file is concise and reference-driven

End execution after Step 4.
