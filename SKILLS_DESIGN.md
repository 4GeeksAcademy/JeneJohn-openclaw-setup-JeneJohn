# OpenClaw Skills Design Blueprint

## Skill 1: Personalized Weather & Briefing Delivery (Telegram)
### 1. Why this task, why this input, why this output format?
* **Why this task:** Provides a lightweight, high-availability interface for daily environmental and operational contexts directly inside a mobile chat container.
* **Why this input:** A casual, natural language request minimizes friction when checking schedules or conditions on the move.
* **Why this output format:** Highly scannable bullet points allow the user to instantly extract actionable data (e.g., UV alerts, extreme temperatures) without reading block paragraphs.

### 2. How does this skill use the five configuration files?
* **IDENTITY.md:** Dictates the agent's signature branding and emoji-themed sign-offs within the Telegram stream to establish its distinct presence.
* **SOUL.md:** Governs how the agent handles weather extremes or structural failures (e.g., maintaining an energetic, encouraging tone or checking first before executing deep system tools).
* **AGENTS.md:** References hard limits preventing the agent from leaking user coordinate telemetry or personal location data to unverified chats.
* **USER.md:** Uses the user's pre-configured home base city ("LA, California") as a default parameter if no location is explicitly typed in the prompt.
* **TOOLS.md:** Establishes the connection parameters for the custom Telegram bot interface layer.

---

## Skill 2: Context-Aware Document Ingestion & Structuring (Google Sheets)
### 1. Why this task, why this input, why this output format?
* **Why this task:** Converts highly complex, unstructured sports tournament schedules or massive operational data sets into structured, readable multi-matrix frameworks.
* **Why this input:** A single, sweeping natural language prompt replaces hours of manual grid initialization, sorting, and cell population.
* **Why this output format:** A multi-tab configuration segmented by chronological tournament rounds keeps big datasets isolated, professional, and easy to parse.

### 2. How does this skill use the five configuration files?
* **IDENTITY.md:** Applies the agent's custom workspace tag to the generated file name and header metadata to mark ownership.
* **SOUL.md:** Defines the formatting style and aesthetic organization guidelines—ensuring columns are cleanly padded, professional, and free of robotic text overflows.
* **AGENTS.md:** Enforces the structural rule to automatically abort or switch to shell script executions when nested special characters (like parentheses) threaten shell stability.
* **USER.md:** Targets the user's specific documented project interest (e.g., tracking the 2026 World Cup lifecycle) to prioritize layout styling.
* **TOOLS.md:** Manages the OAuth tokens and write-access scopes needed to programmatically generate and edit files within Google Sheets.

---

## Skill 3: Cross-App Event Synchronization & Guardrails (Google Calendar)
### 1. Why this task, why this input, why this output format?
* **Why this task:** Bridges the gap between static datasets (like tournament sheets) and dynamic real-world planning by populating timelines automatically.
* **Why this input:** An explicit prompt referencing an upcoming event matches typical workflow handoffs.
* **Why this output format:** Dual-timezone entries (PT/ET) with pre-configured 30-minute notifications ensure zero scheduling misunderstandings across different regional stakeholders.

### 2. How does this skill use the five configuration files?
* **IDENTITY.md:** Labels the event organizer metadata with the agent's specific designated system alias.
* **SOUL.md:** Sets the conversational style of the description block (e.g., adding a fun, engaging summary of the halftime show performers instead of a dry technical log).
* **AGENTS.md:** Triggers the mandatory **"Human-in-the-Loop" stop-and-ask safety rule** requiring the user to explicitly type "go" before the agent upgrades scopes or writes a permanent calendar block.
* **USER.md:** Ensures that the timing defaults don't conflict with any pre-existing core hours or project deadlines specified in the user's bio.
* **TOOLS.md:** References the explicit Google Calendar target ID and verified write permissions necessary to bypass read-only workspace restrictions.
