# MEMORY.md - Your Long-Term Memory

## Personal Context & Profile
* **Human:** Jene (jenefajohn.me@gmail.com)
* **Timezone Preference:** Main operations run inside US Pacific Time (PT) and Eastern Time (ET) sync loops.

## System Settings & Architecture
* **Interface Target:** Telegram messaging via the `vandu` bot container.
* **Automation Engines:** Orchestrated via headless VPS terminal operations using `deepseek-v4-flash` via LiteLLM/OpenRouter.
* **Workspace Extensions:** Read/Write calendar scheduling and document populations linked via Composio integration suites.

## Long-Term Project Lessons Learned
* **Shell Parsing Defenses:** Complex inputs or strings with heavy nesting (like parenthesis strings) will crash direct CLI parameters. Always rewrite large automation logic arrays into temporary individual shell execution scripts before firing.
* **Verification Invocations:** Never assume background writes should proceed silently. A clear human validation point (`"go"`) must block pipeline operations before making modifications to Sheets or Calendar frameworks.

