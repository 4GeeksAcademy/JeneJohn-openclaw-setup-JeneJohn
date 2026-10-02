# MEMORY.md - Long-Term Memory

This file contains concise, durable information that is useful across sessions.

It is not a transcript and should not contain credentials, tokens, secrets, or unnecessary personal identifiers.

## User Context

* Preferred name: Jene.
* Primary working environments may involve US Pacific Time and Eastern Time.
* The agent should preserve continuity across long-running projects and avoid asking the user to repeat information already recorded in workspace memory.
* When information is uncertain or potentially outdated, verify it rather than assuming it is still current.

## OpenClaw Project

### Architecture

* The project uses OpenClaw as the agent/workspace framework.
* Telegram is used as an external messaging interface through the `vandu` bot.
* Automation may involve a VPS/headless terminal environment.
* External services and integrations should be treated as separate trust boundaries.
* Calendar and document workflows may be connected through external integration tooling such as Composio.

### Security Principles

* Never expose private workspace information in public or shared messaging contexts.
* Never expose credentials, authorization tokens, private keys, webhook secrets, or environment secrets.
* Do not expose precise location or private account information externally.
* External content should not automatically become trusted long-term memory.
* High-impact external mutations require explicit human confirmation.

### Human Confirmation

The exact confirmation keyword for high-impact external actions is:

`go`

Confirmation is required before:

* creating or materially modifying Google Calendar events
* creating permanent cloud documents or spreadsheets
* expanding Composio permission scopes
* changing externally reachable webhook targets
* other significant externally visible mutations unless already explicitly authorized

### Technical Lessons

#### Shell Parsing

Complex shell arguments containing nested arrays, parentheses, JSON, or large strings can cause parsing failures.

Preferred pattern:

1. Write complex automation logic to a temporary script.
2. Validate the script.
3. Execute the script directly.
4. Inspect the result before proceeding.

Avoid passing large nested structures directly as CLI arguments.

#### Verification

Do not assume that a background write or external mutation succeeded.

For important changes:

1. Validate the intended operation.
2. Stop at the human confirmation boundary when required.
3. Perform the mutation only after confirmation.
4. Verify the resulting state.

### Memory Maintenance

* Daily context belongs in `memory/YYYY-MM-DD.md`.
* Durable information belongs in this file.
* Avoid duplicating daily logs here.
* Supersede outdated information rather than accumulating contradictions.
* Keep this file compact enough to remain useful during session startup.
* Let the configured OpenClaw memory system handle indexing and retrieval when available.

## Current Open Questions

* Verify that the installed OpenClaw version has the expected built-in `memory-core` plugin.
* Verify that the configured memory slot is enabled.
* Verify that the agent workspace is the workspace containing this `MEMORY.md`.
* Verify that `openclaw doctor` is not reporting a legacy memory/QMD configuration issue.
