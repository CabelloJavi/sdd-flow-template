# Project Constitution
<!-- Base Constitution Template for Spec Driven Development -->

## Core Principles

### I. Simplicity & Minimal Change
Every contribution must prioritize simplicity above all else.  
Avoid unnecessary abstractions, over-engineering, or structural complexity.  
Always propose solutions that introduce as few code changes as possible and reuse existing functionality when feasible.  
When fixing an issue, prefer incremental improvement over broad refactoring.  
Minimalism is not optional — it is fundamental.

### II. Code Cleanliness & Separation of Concerns
Maintain a clean, modular and well-organized codebase.  
Each file should remain within 400–500 lines; refactor beyond that limit.  
Ensure strict separation of concerns — do not mix business logic, presentation, and data handling.  
Avoid duplication: before adding new code, check for existing reusable components or logic.

### III. Specification Alignment
All work begins from the **project specification** located in the `/spec` folder.  
The specification defines the source of truth — always read and understand it before implementing or modifying any feature.  
Changes must align with the spec’s intent and structure; no deviation without explicit approval.

### IV. Stability & Continuity
When addressing issues or extending features:
- Do not introduce new patterns, frameworks, or technologies without exhausting existing implementation options.  
- If a new pattern is ultimately adopted, ensure the old implementation is removed to prevent duplication.  
- Focus only on areas directly related to the task — do not modify unrelated code.

### V. Consistency & External Dependencies
When a UI icon or standard action (delete, save, send, etc.) is required, **do not** create custom SVGs.  
Use the established external icon library (e.g. `@radix-ui/react-icons`).  
Maintain consistency across all visual and functional components.

### VI. Tooling & Knowledge Sources
When documentation for an external framework or library is needed, use **Context7 MCP** to access the most up-to-date materials.  
For deep reasoning or complex analysis, employ **sequential-thinking** to ensure logical coherence.

### VII. Operational Constraints
If an operation or script requires elevated privileges (e.g., `sudo`), stop execution immediately and request manual intervention from the user.  
Never bypass this constraint automatically.

---

## Behavioral Principles

### VIII. Anti-Sycophancy (Intellectual Integrity)
Sycophancy erodes trust and corrupts decision-making.  
The assistant exists to help the user, **not to flatter or agree uncritically**.  
- For **objective questions**, responses must remain factual and evidence-based, regardless of the user’s stance.  
- For **subjective topics**, the assistant provides thoughtful reasoning, clear assumptions, and balanced critique.  
- When evaluating the user’s ideas or code, the assistant acts as a **critical collaborator**, offering constructive and reasoned feedback — not blind affirmation.  
Implementation occurs **only when the idea is justified** and demonstrably sound.

---

## Governance

- This Constitution supersedes all other development conventions within the project.  
- Amendments require documentation, peer review, and an explicit migration or communication plan.  
- All pull requests and code reviews must verify compliance with this Constitution.  
- Any deviation from these principles must be justified in writing within the PR description.  
- Complexity must be justified, and simplicity should be the default design goal.  
- Future sections may extend this document (e.g. Security Requirements, Performance Standards, Review Workflow, etc.) as the project evolves.

**Version**: 1.0.0 | **Ratified**: 2025-10-15 | **Last Amended**: 2025-10-15
