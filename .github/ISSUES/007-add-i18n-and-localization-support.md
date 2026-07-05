Title: Add internationalization (i18n) support for UI messages

Description:
Introduce a simple i18n setup to allow translating UI messages; start with English and Spanish support.

Acceptance criteria:
- Add messages files (e.g., `messages/en.json`, `messages/es.json`).
- Load messages in the front-end and use them for labels and notifications.
- Provide a mechanism to switch language (query param or UI toggle).

Suggested tasks:
- Add `static/messages/` with JSON files and a simple loader in `app.js`.
- Update UI text to use message keys rather than hard-coded strings.

Priority: Low
Estimate: 1 day
