# Security and privacy

Daheim is a client-side household planning tool, not a secure vault.

- Inventory and checklist data are stored in the browser's IndexedDB on the current device and origin.
- No account, server-side database, analytics, advertising, or remote API is used by the app.
- The public repository contains application source code only. Never commit household backup JSON files or other personal information.
- Anyone with access to the browser profile or an exported backup may be able to read the household data.
- Use device encryption and a screen lock, and store exported backups privately.
- Clearing browser storage, changing browser profiles, or uninstalling/clearing app data may remove local records. Keep regular backups.
