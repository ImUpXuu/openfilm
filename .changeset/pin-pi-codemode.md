---
"@openfilm/desktop": patch
---

The app's own agent starts again: the packaged app had `@earendil-works/pi-coding-agent` 1.1.0 beside `pi-codemode` 1.2.0, which no longer exports `MCP_TYPESCRIPT_PREAMBLE`, so the agent crashed on start and every "Own key" message ended with "ACP connection closed". `pi-codemode` is now a direct dependency at 1.1.0.
