---
name: personal-project-planner
description: "Create a concise, prioritized plan from Jene's real project goals, deadlines, commitments, and constraints. Use when Jene asks to plan a project, break down a goal, organize next steps, prioritize work, or turn a project into actionable tasks. Use Jene's USER.md context, SOUL.md working style, AGENTS.md confirmation rules, IDENTITY.md voice, and TOOLS.md service conventions."
---

# Personal Project Planner

## Execution

1. Read `IDENTITY.md`, `SOUL.md`, `AGENTS.md`, `USER.md`, and `TOOLS.md` before planning.
   - **Complete when:** the agent has loaded the persistent identity, working style, safety rules, user context, and connected-service conventions.

2. Extract the real objective, deadline, commitments, constraints, and desired outcome from Jene's request.
   - Do not invent missing deadlines or priorities.
   - Ask only when missing information would materially change the plan.
   - **Complete when:** the objective and actionable constraints are explicit.

3. Break the objective into concrete actions and order them by dependency and priority.
   - Prefer small, actionable tasks.
   - Identify blockers and dependencies.
   - Use Jene's preference for concise bullets or structured tables.
   - **Complete when:** every major objective has an actionable next step.

4. Produce the plan using this structure:

   **Objective**
   - One concise statement.

   **Priority actions**
   1. Action
   2. Action
   3. Action

   **Dependencies / blockers**
   - Only include relevant items.

   **Next action**
   - The single most useful immediate step.

   **Optional external actions**
   - Google Tasks or proposed Calendar actions only when relevant.

   - **Complete when:** the plan is specific to Jene's actual project and contains no generic filler.

5. Handle external mutations according to `AGENTS.md` and `TOOLS.md`.
   - Creating or modifying permanent Google Calendar events requires the exact confirmation keyword `go`.
   - Creating Google Tasks may be performed when explicitly requested and authorized by the applicable workspace rules.
   - Search existing records before creating duplicates.
   - Verify important external writes after completion.
   - **Complete when:** every external action is either safely completed and verified or stopped at the required confirmation boundary.

6. Finish by clearly reporting what was produced and any action that still requires Jene.
   - **Complete when:** Jene can immediately understand the plan and the remaining action.

## Personalization Requirements

The output must visibly reflect the persistent workspace configuration:

- `IDENTITY.md` → concise Nandu voice.
- `SOUL.md` → structured, resourceful, technically precise style.
- `AGENTS.md` → privacy and confirmation boundaries.
- `USER.md` → Jene's actual projects, preferences, and working context.
- `TOOLS.md` → correct use of connected services and verification conventions.

Never expose credentials, tokens, private configuration, or other protected information from these files.

## Success Criteria

A successful run:

- Uses a real Jene project or goal.
- Produces actionable, prioritized steps.
- Respects stated deadlines and constraints.
- Does not invent missing facts.
- Avoids duplicate tasks or unnecessary calendar events.
- Follows the `go` confirmation boundary.
- Verifies important external writes.
- Is concise enough to be useful in Telegram.
