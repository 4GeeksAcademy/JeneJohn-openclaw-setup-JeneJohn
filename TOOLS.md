# TOOLS.md - Local Notes

This file details the environment-specific configurations and active service connections unique to Nandu's deployment environment.

## Integration Providers

### Composio Tool Suite
* **Google Workspace API:** Active connection with explicit Read/Write permissions granted for Google Sheets and Google Calendar pipelines.
* **Default Spreadsheet Target:** FIFA World Cup 2026 Schedule multi-tab project tracking ledger.
* **Default Calendar Target:** Primary user work calendar synced across Eastern Time (ET) and Pacific Time (PT).

## Local Systems & Infrastructure

### Remote Server Execution (SSH)
* **Active Host Instance:** root@bc-vps-204 (IP: 157.245.139.131)
* **Execution Interface:** Headless Linux terminal runtime.
* **System Environment:** Script-based task handlers deployed to safely manage terminal string expansions and avoid parenthesis parsing crashes.

## Chat Ecosystem Interfaces

### Telegram Integration
* **Bot Target:** `vandu` bot (Primary human-to-agent conversational messaging client).
* **Bot Controller:** `BotFather` token registry hook.
* **User Target ID:** Telegram User ID 8839870265
* **Security Verification Channel:** OpenClaw numeric authentication and pairing string validation routines (`7B2H7BUM`).

## Model & Orchestration Settings

### Inference Framework
* **Orchestration Layer:** LiteLLM integrated with OpenRouter endpoints.
* **Primary Language Model:** `deepseek/deepseek-v4-flash`


