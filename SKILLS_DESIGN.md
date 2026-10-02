# OpenClaw Skills Design Blueprint

## Skill 1: Cross-Platform Chat Automation (Telegram ➔ Tools)
### 1. What does this skill do?
Provides a natural language interface over Telegram (`vandu` bot) powered by a lightweight LLM (`deepseek-v4-flash`), allowing users to query live web APIs (like weather systems) and securely pair external application tokens using secure numeric and alphanumeric verification pins.

### 2. What input does the agent need?
* **Runtime Input:** Conversational prompts via Telegram or terminal hooks (e.g., "Whats the weather like tomorrow?") and system initialization streams (e.g., `/start` commands and `openclaw pairing approve` triggers).
* **Static Context:** Secure session handling (`litellm/openrouter`), configuration protocols, and device location logs provided dynamically during user setup (e.g., "LA, California").

### 3. What does a good output look like?
* **Format:** Real-time, cleanly bulleted chat summaries breaking down explicit metrics (High/Low temperatures, UV Indices, Sunshine duration, and weather context warnings).
* **Destination:** Active Telegram user chat interface.
* **Success Metric:** Zero-latency intent recognition that converts conversational user text into structured, tool-compatible parameters while handling multi-attempt failure exceptions gracefully.

---

## Skill 2: Structured Document Orchestration (Composio ➔ Google Sheets)
### 1. What does this skill do?
Parses unstructured event data or complex multi-stage tournament plans (such as the FIFA World Cup 2026), builds custom spreadsheet matrix configurations, and fully populates tabular tracking logs down to localized dates, matchups, venues, and stage results.

### 2. What input does the agent need?
* **Runtime Input:** Direct instructions to generate schedules or datasets (e.g., "make a google sheets sheet that has the schedule of the games in FIFA Worldcup2026").
* **Static Context:** Scripted data schemas handled via automated shell scripting execution blocks to avoid parsing errors (such as nested punctuation/parentheses shell issues).

### 3. What does a good output look like?
* **Format:** A fully formatted Google Spreadsheet containing specialized, logically grouped tab views (`Group Stage`, `Round of 32`, `Round of 16`, `Quarterfinals`, `Semifinals`, `Final`).
* **Structure:** High-scannability column grids displaying chronological matchdays, operational group letters, matchup pairings, chronological kickoff times, and stadium venue metrics.
* **Destination:** Dynamically generated sheets hosted via the Google Drive/Sheets workspace.
* **Success Metric:** Complete data ingestion across dozens of rows spanning multiple worksheet categories, leaving no unhandled formulas or empty stages.

---

## Skill 3: Synchronized Workspace Event Scheduling (Composio ➔ Google Calendar)
### 1. What does this skill do?
Automates the lifecycle of calendar event curation by verifying read/write permissions via OAuth flows and converting raw, text-based schedules into highly detailed calendar milestones.

### 2. What input does the agent need?
* **Runtime Input:** Simple explicit intents (e.g., "Create a calendar event for the FIFA WORLDCUP 2026 FINAL game") alongside human-in-the-loop authorization signals ("go").
* **Static Context:** Automated checks for existing authentication scopes to verify that the target calendar has direct write access rather than restrictive read-only profiles.

### 3. What does a good output look like?
* **Format:** Comprehensive Google Calendar block with optimized descriptive summaries (e.g., halftime show updates featuring specific performers).
* **Structure:** Automated timezone translation mapping localized match times into dual references (e.g., 12:00 PM PT / 3:00 PM ET) anchored to a verified physical stadium location.
* **Destination:** Target user's primary Google Calendar database.
* **Success Metric:** Seamless generation of calendar blocks containing complete time spans, accurate location geocoding text, and built-in contextual alerts (e.g., 30-minute system notification reminders) without duplicate creations.

