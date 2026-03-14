# Development Workflow Notes

This directory contains internal development notes for maintaining the Janus public site repository.

## Scope control

- Prefer small, reviewable commits.
- Stage only the intended files.
- Keep public-site changes separate from specification work.

## Evidence and review

- Treat `git diff` as the primary evidence artifact for content and integration changes.
- Validate links and navigation paths after changes that affect routing.
- Keep the working tree clean after each publish step.

## Tool Friction Reduction

Editor confirmation prompts (e.g., repetitive “Allow” approvals before actions such as commits, file writes, or command execution) may be reduced during development **provided that Janus governance guarantees remain intact**.

Reducing tool prompts must not weaken the governance boundary:

- Scope control remains explicit (only intended files staged and committed).
- Evidence remains reviewable (diffs, logs, and public artifacts remain inspectable).
- Closed-loop accountability remains enforced (human review/approval where required).

Tooling convenience is not a substitute for governance.
