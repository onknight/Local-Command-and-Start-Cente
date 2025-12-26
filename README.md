Based on your progress and the code in Peak.html, here is the updated README.md for Version 1.3.6. This version marks the completion of the Credential Security phase and sets the stage for the transition to a standalone desktop application.

Local Command and Start Center (LCSC)
Version 1.3.6 | The Secure Vault & Data Integrity Update

🎯 Project Definition
The LCSC is a private, high-density navigation hub. It acts as a "Single Pane of Glass" for managing local homelab services and internal IP addresses without the privacy risks of cloud-based start pages.

The Philosophy
Stealth First: Admin tools and sensitive vault data remain invisible until specifically invoked, maintaining a minimalist aesthetic.

Local First: All configuration, visual data, and imported vault credentials stay in your browser's localStorage.

Zero Friction: A single-file HTML solution that provides enterprise-level dashboarding without a backend.

🚀 Key Features
Integrated Site Vault: A local credential manager that allows you to browse and search imported logins without leaving the dashboard.

Smart CSV Parser: Advanced logic that identifies "Site Name," "Username," and "Password" columns automatically to prevent data mapping errors.

Dynamic HUD (Heads-Up Display): A sliding interface that presents credentials and site names with one-click "Copy to Clipboard" functionality.

Stealth Management: Shortcut editing and deletion controls are hidden until the Alt key is engaged.

Data Recovery Engine: Full JSON backup and restoration suite to move your entire environment (including wallpaper positions) between devices.

⌨️ System Registry (Shortcut Guide)
Vault Controls
📂 BROWSE VAULT: Open the searchable credential explorer.

Esc: Instantly close the Vault, HUD, or Help Overlay.

Alt + F2: Vault Purge – Permanently wipes all imported CSV data (added in v1.3.6).

Management (Hold Alt)
Alt + N: Create New Shortcut.

Alt + E: Edit Shortcut (while mouse-hovering).

Alt + D: Delete Shortcut (while mouse-hovering).

Visuals & Environment
Alt + B: Change Wallpaper (Upload Image).

Alt + F1: Reset All Visuals & Nudge Data.

Alt + Arrow Keys: Nudge Background Position (10px steps) for pixel-perfect alignment.

🗺 Development Roadmap
✅ Stage 1: Interface & Stealth UI (COMPLETE)
High-density grid, search integration, and stealth controls.

✅ Stage 2: Credential Security (COMPLETE)
Local Vault integration, CSV parsing engine, and Secure HUD display.

⏳ Stage 3: Desktop Standalone (PLANNED)
Electron.js Wrapper: Converting the single-file HTML into a cross-platform desktop app.

System Tray Minimization: Running the Command Center as a persistent background utility.

Global Hotkeys: Invoking the Command Center from anywhere in the OS.

Build v1.3.6 Stable | Developed by Tom | Documentation by Gemini
---

## 4. Development Roadmap

| Phase   | Milestone              | Primary Technologies        | Status       |
| ------- | ---------------------- | --------------------------- | ------------ |
| Stage 1 | Interface & Stealth UI | HTML5, CSS3, JavaScript     | **Complete** |
| Stage 2 | Credential Security    | Proton Pass API Integration |**Complete**     |
| Stage 3 | Desktop Standalone     | Electron.js Framework       | Planned      |
| Stage 4 | Server Hosting         | Docker, Nginx (Homelab)     | Planned      |

---

## 5. Data Integrity and Recovery

All data, including shortcuts and backgrounds, is stored locally in the browserâ€™s `localStorage`.

**Important:**

* Clearing browser cache or site data will erase all user configurations.
