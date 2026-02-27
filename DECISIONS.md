# DECISIONS.md – Overrides & Important Choices

This file records important decisions that should affect automation, especially cron jobs and sub-agents.

Use it to log things like:
- "Cancel that follow-up to customer X, already handled manually."
- "Pause all MA3DPrints marketing outreach until DATE."
- "Stop sending reminder emails about OFFER Y."

## Format

Keep entries short and dated. Examples:

- 2026-02-27 – Cancel any scheduled follow-ups related to lead #123 (handled manually).
- 2026-02-27 – Do not send any automated emails about the old pricing page; we’re revising pricing.
- 2026-03-01 – Pause all social posting crons until I say resume.

Automation rules:
- Any cron or sub-agent that takes **external action** (emails, DMs, posts, calls, etc.) should scan this file first.
- If an entry clearly conflicts with the planned action, **abort** and log why instead of proceeding.

