# OpenClaw Skills Design Blueprint

This project implements two custom OpenClaw skills focused on Jene's actual productivity workflows. Both skills use the persistent agent configuration in `IDENTITY.md`, `SOUL.md`, `AGENTS.md`, `USER.md`, and `TOOLS.md` rather than behaving like generic prompts.

---

## Skill 1: Personal Project Planner

### 1. What does this skill do?

Turns a user's project or goal into a concise, prioritized action plan and, when requested, converts the actionable items into Google Tasks or proposed Google Calendar blocks.

### 2. What input does the agent need?

**Runtime Input:**

* A real project, goal, deadline, or set of commitments from Jene.
* Optional constraints such as available time, deadline, priority, or preferred schedule.

Example:

> "Help me plan the next steps for my OpenClaw assignment. I want to finish the two skills and test them this week."

**Static Context from the five configuration files:**

* `IDENTITY.md` provides Nandu's identity and concise operational voice.
* `SOUL.md` requires structured output, proactive problem solving, and careful handling of external writes.
* `AGENTS.md` defines the `go` confirmation requirement for high-impact external changes.
* `USER.md` provides Jene's current projects, technical preferences, and preference for concise bullet/table-based output.
* `TOOLS.md` defines when to use Google Tasks and Google Calendar and the conventions for external writes.

### 3. What does a good output look like?

**Format:**

* Short project objective.
* Prioritized action list.
* Dependencies or blockers.
* Suggested next action.
* Optional proposed calendar/task actions.

**Destination:**

* Normally returned in the conversation.
* Google Tasks when the user asks to create actionable tasks.
* Google Calendar only after required confirmation for permanent event creation or modification.

**Success Criteria:**

* The plan is specific to Jene's project rather than generic advice.
* Tasks are actionable and ordered logically.
* Existing constraints and deadlines are respected.
* No duplicate tasks or unnecessary calendar events are created.
* External mutations stop at the `go` confirmation boundary when required.
* Any completed external write is verified.

---

## Skill 2: Structured Learning & Project Log

### 1. What does this skill do?

Converts Jene's rough learning notes, technical discoveries, decisions, and project progress into a concise structured entry and appends it to a persistent Google Doc.

### 2. What input does the agent need?

**Runtime Input:**

* Rough notes, lessons learned, project progress, technical discoveries, or decisions.

Example:

> "Today I figured out that OpenClaw was using the wrong workspace, so memory wasn't indexing the repo. I changed the workspace to the GitHub repo and disabled semantic search because no OpenAI key is configured."

**Static Context from the five configuration files:**

* `IDENTITY.md` establishes Nandu's precise, technical communication style.
* `SOUL.md` instructs Nandu to be resourceful, structured, privacy-conscious, and concise.
* `AGENTS.md` establishes memory hygiene, privacy rules, and verification requirements.
* `USER.md` provides Jene's active OpenClaw project context and technical preferences.
* `TOOLS.md` defines Google Docs usage, Drive conventions, and verification requirements.

### 3. What does a good output look like?

**Format:**

Each entry should contain:

* **Date**
* **Project**
* **What changed**
* **Key learning**
* **Decision**
* **Next step**
* **Relevant technical notes**, when useful

The entry should be concise and easy to scan later.

**Destination:**

* The structured result is shown to Jene for review.
* After confirmation/authorization where required, the finalized entry is appended to the designated Google Doc.
* Existing document structure should be preserved.

**Success Criteria:**

* The notes accurately reflect the user's actual input.
* Important technical decisions are preserved without unnecessary narrative.
* The output uses Jene's preferred concise structure.
* No credentials, tokens, private identifiers, or other sensitive information are recorded.
* The correct existing document is used rather than creating an unnecessary duplicate.
* The Google Docs write is verified after completion.
* The resulting entry is useful as future project context rather than being a raw transcript.

---

## Why These Two Skills

### Personal Project Planner

Jene frequently works on technical projects with multiple steps, dependencies, and external services. This skill demonstrates the agent's ability to combine persistent user context with structured planning and controlled external actions.

### Structured Learning & Project Log

The OpenClaw project involves experimentation, configuration changes, troubleshooting, and technical decisions. This skill demonstrates persistent context management while providing a concrete verified Google Workspace output.

Together, the skills demonstrate:

* Persistent configuration-driven behavior.
* Personalized outputs based on `USER.md`.
* Consistent personality and formatting from `SOUL.md` and `IDENTITY.md`.
* Safety and confirmation boundaries from `AGENTS.md`.
* Correct use of connected services from `TOOLS.md`.
* Real external-service output rather than terminal-only prompts.
* Verification after external mutations.
