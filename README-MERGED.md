# MKMODZ Abbas MD — 101 Commands + Web Pairing

This build keeps the original Mini Bot web pairing/deployment architecture while using the 101-command `main.js` engine.

- Web pairing page is preserved at `/`.
- User enters a WhatsApp number and receives a pairing code.
- No `SESSION_ID` input and no manual `creds.json` upload are required.
- Per-number sessions are created automatically under `session/session_<number>` and persisted through the existing MongoDB session system.
- Existing Railway/Express startup and deployment flow is preserved.
- Legacy command registry/plugins are not used for message commands.
- The 101-command `main.js` handles incoming messages and group events.
