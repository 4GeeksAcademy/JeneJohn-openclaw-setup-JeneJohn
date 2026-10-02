---
name: personalized-weather-briefing
description: "Provides a lightweight, high-availability interface for daily environmental and operational contexts directly inside a Telegram mobile chat container. Use when Jene asks for weather data, daily briefings, or schedule conditions. Uses Jene's USER.md context, SOUL.md working style, AGENTS.md privacy rules, IDENTITY.md voice, and TOOLS.md Telegram bot parameters."
---

# Personalized Weather & Briefing Delivery (Telegram)

## Design Blueprint

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

## Execution Framework

1. **Preflight Context Verification**
   - Read `IDENTITY.md`, `SOUL.md`, `AGENTS.md`, `USER.md`, and `TOOLS.md` before processing the prompt.
   - **Complete when:** The agent registers Jene's operational state, targets the active Telegram user ID, and establishes location contexts.

2. **Parameter Ingestion & Default Handling**
   - Parse the casual, natural language incoming request for specific location metrics.
   - If no explicit location is typed in the prompt, pull the default home base parameter ("LA, California") from `USER.md`.
   - **Complete when:** The target geo-coordinates or region parameters are finalized.

3. **Data Retrieval and High-Scannability Formatting**
   - Query authorized live environmental and weather systems using parameters established via `TOOLS.md`.
   - Compress massive raw API streams into highly scannable bullet points detailing explicit variables (High/Low temperatures, UV indices, extreme conditions, and sunshine duration metrics).
   - Apply the distinct signature branding and emoji parameters dictated by `IDENTITY.md` and `SOUL.md` (maintaining an energetic tone even during system extreme weather faults).
   - **Complete when:** The final text transmission block is formatted cleanly without walls of block paragraph narrative text.

4. **Privacy Guardrails & Transmission Verification**
   - Intercept the transmission package before it routes to ensure zero user data leaks occur.
   - Ensure hard safety limits from `AGENTS.md` block any raw user coordinate telemetry, email definitions, or credentials from leaking into unverified endpoints.
   - Route the final clean payload straight to the custom Telegram bot interface layer destination channel.
   - **Complete when:** The real-time brief is safely printed inside the active chat surface container.

---

## Success Criteria

A successful run:
- Resolves location context smoothly using fallback profiles if necessary.
- Avoids dense corporate phrasing and utilizes Nandu's emoji-themed signature sign-offs.
- Strictly adheres to the zero-leak boundary for private coordinate or token data.
- Keeps outputs optimized, lightweight, and fast for delivery over mobile interfaces.
