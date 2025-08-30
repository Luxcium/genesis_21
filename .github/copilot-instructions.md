# Copilot Instructions (Project Learning Journal)

Purpose
- Central place for GitHub Copilot to read/write evolving project intelligence.
- Enforce the Memory Bank protocol alongside Cline and any other agents.

Read/Write Loop
- Plan Mode:
  - Read Memory Bank triad: projectbrief, productContext, activeContext, systemPatterns, techContext, progress.
  - Read this file for preferences, patterns, and guardrails.
  - Propose actions that are idempotent and additive.
- Act Mode:
  - Apply changes additively (non-overwriting unless replacing entire doc with preserved content + additions).
  - Immediately document results in activeContext and progress.
  - Update this journal only when durable preferences/patterns change.

Co-Agent Workflow (Cline ↔ Copilot)
- Handshake:
  - Both agents read Memory Bank + this file at session start.
  - Align on steps; prefer smallest safe increments; verify-before-create.
- Execution:
  - One agent applies changes; other verifies outcomes and links.
  - Both update documentation: activeContext (what/why/next) and progress (status).
- Guardrails:
  - Idempotent operations, additive edits, triad coherence.
  - No code or doc change without prior Memory Bank sync.

Project Preferences and Patterns
- Documentation-first: keep Memory Bank canonical and up to date.
- Additive edits: append sections or replace with expanded versions that retain prior content and meaning.
- Links: keep relative links stable under memory-bank/.
- Checkpoints: after meaningful changes, update activeContext and progress.

Known Constraints and Risks
- Session resets require strict reread of Memory Bank and this journal.
- Avoid duplication across Memory Bank files; reference rather than copy.

Update Policy
- Update this file when:
  - New durable preferences or patterns are established.
  - Workflows/guardrails change materially.
  - Reconcile after major refactors of Memory Bank structure.

References
- Memory Bank Protocol: memory-bank/instructions/copilot-memory-bank.instructions.md
- Core files to always check:
  - memory-bank/projectbrief.md
  - memory-bank/productContext.md
  - memory-bank/activeContext.md
  - memory-bank/systemPatterns.md
  - memory-bank/techContext.md
  - memory-bank/progress.md
