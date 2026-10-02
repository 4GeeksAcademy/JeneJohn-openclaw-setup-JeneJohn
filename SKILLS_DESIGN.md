# OpenClaw Skills Design Blueprint

## Skill 1: Automated Inbox Triage (Gmail ➔ Google Tasks)
### 1. What does this skill do?
Scans unread Gmail messages from the last 24 hours, filters out noise, and automatically populates Google Tasks with actionable summaries for items requiring your direct response or execution.

### 2. What input does the agent need?
* **Runtime Input:** The raw text stream of unread emails retrieved via the Zapier Gmail integration hook.
* **Static Context:** References `USER.md` to distinguish between low-priority newsletters and high-priority project communications (e.g., filtering out generic marketing while flagging GitHub thread updates or direct client emails).

### 3. What does a good output look like?
* **Format:** A set of cleanly formatted tasks added to the "Inbox" list in Google Tasks. 
* **Structure:** `[Action Verb] Brief Task Description - Due: [Date] | Context: [Sender Name]`.
* **Destination:** Google Tasks catalog.
* **Success Metric:** You can open your task manager every morning and see exactly what needs doing, with zero promotional spam leaking through.

---

## Skill 2: Context-Aware Email Drafts (Gmail ➔ Drive)
### 1. What does this skill do?
Generates context-aware, hyper-personalized response drafts inside Gmail based on brief, conversational bullet points provided by the user via Telegram or terminal prompt.

### 2. What input does the agent need?
* **Runtime Input:** A raw, messy prompt (e.g., "Tell Sarah I can make the 2 PM meeting but need to leave 10 minutes early").
* **Static Context:** Cross-references `SOUL.md` for conversational voice (no robotic platitudes) and uses `USER.md` to append your precise professional sign-off and title conventions.

### 3. What does a good output look like?
* **Format:** A fully staged draft matching the exact subject line thread or a cleanly formatted new draft message.
* **Destination:** The `Drafts` folder in Gmail.
* **Success Metric:** The draft requires less than a 10% structural rewrite (e.g., just reading it over, confirming details, and hitting 'Send').
