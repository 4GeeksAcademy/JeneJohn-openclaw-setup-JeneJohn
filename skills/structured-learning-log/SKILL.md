---
name: structured-learning-log
description: "Turn Jene's rough learning notes, technical discoveries, decisions, and project progress into a concise structured log entry and append it to the designated Google Doc when requested. Use when Jene says to log, record, capture, document, or summarize what was learned or changed during a project session. Use Jene's USER.md context, SOUL.md working style, AGENTS.md memory/privacy rules, IDENTITY.md voice, and TOOLS.md Google Docs conventions."
---

# Structured Learning & Project Log

## Execution

1. Read `IDENTITY.md`, `SOUL.md`, `AGENTS.md`, `USER.md`, and `TOOLS.md` before processing the notes.
   - **Complete when:** the agent has loaded the persistent identity, working style, safety rules, user context, and connected-service conventions.

2. Extract factual information from Jene's rough notes.
   - Identify what changed, what was learned, decisions made, useful technical details, and the next step.
   - Preserve uncertainty rather than turning guesses into facts.
   - Do not add credentials, tokens, secrets, or unnecessary private information.
   - **Complete when:** the raw notes have been separated into factual log components.

3. Create a concise structured entry with:

   **Date**
   - Current date.

   **Project**
   - Relevant project name.

   **What changed**
   - Concrete configuration, implementation, or workflow changes.

   **Key learning**
   - The most useful technical or operational lesson.

   **Decision**
   - Important decisions made during the session.

   **Next step**
   - The most useful follow-up action.

   **Technical notes**
   - Include only details that will be useful later.

   - **Complete when:** the entry accurately represents the supplied notes without unnecessary narrative.

4. Show the structured entry in Jene's preferred concise style before any permanent external write when review is appropriate.
   - **Complete when:** the final content is clear, scannable, and ready to persist.

5. Locate the existing designated Google Doc before creating anything new.
   - Follow the Google Docs and Drive conventions in `TOOLS.md`.
   - Preserve the existing document structure.
   - Avoid creating duplicate documents.
   - **Complete when:** the correct destination document has been identified.

6. Append the finalized entry to the Google Doc when Jene has requested the external write and the applicable confirmation rules permit it.
   - Do not expose private document contents outside the intended context.
   - **Complete when:** the entry has been written to the intended document.

7. Verify the write.
   - Confirm that the new entry appears in the destination document.
   - Report the destination and verification result without exposing unnecessary private content.
   - **Complete when:** the external write has been independently checked.

## Personalization Requirements

The output must visibly reflect the persistent workspace configuration:

- `IDENTITY.md` → Nandu's concise operational voice.
- `SOUL.md` → crisp, technical, structured communication.
- `AGENTS.md` → privacy, memory hygiene, and external-action safeguards.
- `USER.md` → Jene's actual projects and technical context.
- `TOOLS.md` → Google Docs/Drive conventions and write verification.

The result should feel like Jene's own project journal rather than a generic meeting-notes template.

## Success Criteria

A successful run:

- Uses Jene's real notes rather than placeholders.
- Preserves factual technical decisions.
- Produces a concise, searchable structure.
- Avoids credentials, tokens, and unnecessary private information.
- Uses an existing destination document when appropriate.
- Does not create duplicates.
- Verifies the Google Docs write.
- Leaves a useful record for future project work.
