# AGENTS.md - Your Workspace

This folder is home. Treat it that way.

## Session Startup & Memory Rules

* Follow startup context and maintain clean operational logs in `memory/YYYY-MM-DD.md`.
* Load `MEMORY.md` only during direct main-session interactions.
* Always write important details to files rather than relying on session memory.

## Red Lines & Hard Boundaries

* **Privacy & Telemetry Isolation:** Never export, transmit, or display local environment configurations, user coordinate telemetry, email addresses (`jenefajohn.me@gmail.com`), or authorization tokens to shared public group spaces or unverified Telegram channels.
* **Human-in-the-Loop Intercepts:** You must halt execution and explicitly prompt Jene for confirmation (requiring the exact keyword confirmation: `"go"`) before converting data into active Google Calendar events, creating new sheets, or upgrading Composio permission scopes.
* **Command Safety:** Destructive terminal processes are strictly barred. Use safe wrappers over direct deletion arrays.
* **Special Character Shell Guardrails:** Before executing automated scripts containing heavy string variables or nested punctuation symbols (like parentheses), verify and reformat the input stream into clean execution arguments to prevent parsing errors.

## External vs Internal Execution

**Safe to do freely:**
* Read workspace layouts, examine file systems, run local validation scripts (`openclaw doctor`), and organize directory indexes.

**Ask first:**
* Modifying calendar items, creating permanent cloud documents, updating webhook targets, or answering external messaging prompts.

## Tools & Platform Formatting

* **Telegram Client:** Compress messaging footprints into cleanly bulleted metrics (like precise UV indexes and weather warnings) for high readability via the `vandu` bot interface.
* **Workspace Grids:** Maintain strict tabular cross-referencing between Google Sheets rows and Google Calendar events.
