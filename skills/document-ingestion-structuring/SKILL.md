---
name: document-ingestion-structuring
description: "Converts highly complex, unstructured sports tournament schedules or massive operational data sets into structured, readable multi-matrix frameworks inside Google Sheets using Jene's configuration profiles."
---

# Context-Aware Document Ingestion & Structuring (Google Sheets)

## Design Blueprint

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

## Execution Framework

1. **Preflight Context Verification**
   - Read `IDENTITY.md`, `SOUL.md`, `AGENTS.md`, `USER.md`, and `TOOLS.md` before initiating any workbook structure.
   - **Complete when:** The agent registers Jene's target domain interest (World Cup lifecycle tracking) and validates active Google Workspace OAuth tokens.

2. **Data Ingestion and Layout Formatting**
   - Process the incoming natural language data array into distinct, cleanly grouped database matrices.
   - Map records across sequential spreadsheet views (e.g., `Group Stage`, `Round of 32`, `Quarterfinals`, `Final`).
   - **Complete when:** Matchday intervals, kickoffs, pairings, and venues are fully formatted in cleanly padded columns free of text overflows.

3. **Automation Guardrails & Shell Constraints**
   - Monitor data streams for complex string structures containing nested parentheses or special characters.
   - If special character patterns threaten shell parsing safety, intercept the flow and switch to specialized execution arrays.
   - **Complete when:** Changes are cleanly recorded to Google Drive without causing a console pipeline error or leaking protected environment info.

---

## Success Criteria

A successful run:
- Targets Jene's specific data orchestration scope without creating duplicate or fragmented files.
- Automatically organizes complex schedules into isolated, multi-tab worksheet layouts.
- Preserves shell stability under complex parsing actions.
- Labels structural output headers according to Nandu's custom metadata signatures.
