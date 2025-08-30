# Copilot Guardrails

Scope

- Treat `memory-bank/` as canonical context. Read instructions before writing memory files.

Standards

- TypeScript-first posture with TSDoc for public APIs.
- Node.js baseline: 22+.
- ESLint flat config expected; all fixable rules as warnings.
- Integrate Prettier via `eslint-config-prettier` (no plugin).

Agent Guidance

- Use VS Code triad locations from `.vscode/settings.json`.
- Do not overwrite existing files unless explicitly instructed.
- Keep actions idempotent; prefer additive changes.
