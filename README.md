## 1. Project Scope and Utility

The **Local Command and Start Center** is a privacy-first, high-density dashboard designed to consolidate daily web tools and local network services, including homelab environments.

It bypasses standard browser â€œnew tabâ€ limitations by supporting **unlimited shortcuts** and employing a **Stealth UI model**. All administrative controls are hidden and accessible only via keyboard commands, ensuring a clean interface.

---

### 2.1 Global Commands

* `?` : Toggle the Help / Shortcuts Legend overlay
* `Alt + N` : Create a new shortcut
* `Alt + B` : Open file browser to set a custom background image
* `Alt + R` : Reset background to `background.png` and recenter
* `Alt + Arrow Keys` : Nudge background image position (2% increments)

---

### 2.2 Contextual Commands

*(While the mouse is hovering over a shortcut)*

* `Alt + E` or `Alt + Enter` : Edit the selected shortcutâ€™s name or URL
* `Alt + D` : Delete the selected shortcut


---

## 3. Core System Logic

### 3.1 Smart Protocol Detection

The system automatically handles protocols to ensure correct service resolution:

* **Local Network**: URLs with `192.168.*`, `10.*`, `127.*`, or `*.local` are prefixed with `http://`.

* **Standard Web**: Domains default to `https://`.

* **Manual Override**: User-defined protocols (e.g., `ftp://`) are preserved as entered.

---

### 3.2 Background Persistence Engine

Background images are stored as Base64 data in the browserâ€™s `localStorage`.

* **Storage**: Images are encoded and saved, independent of the original file location.
* **Positioning**: Any adjustments to the background position are saved and retained across sessions.
* **Reset**: Resetting the background returns the image and positioning to default.

---

## 4. Development Roadmap

| Phase   | Milestone              | Primary Technologies        | Status       |
| ------- | ---------------------- | --------------------------- | ------------ |
| Stage 1 | Interface & Stealth UI | HTML5, CSS3, JavaScript     | **Complete** |
| Stage 2 | Credential Security    | Proton Pass API Integration | Planned      |
| Stage 3 | Desktop Standalone     | Electron.js Framework       | Planned      |
| Stage 4 | Server Hosting         | Docker, Nginx (Homelab)     | Planned      |

---

## 5. Data Integrity and Recovery

All data, including shortcuts and backgrounds, is stored locally in the browserâ€™s `localStorage`.

**Important:**

* Clearing browser cache or site data will erase all user configurations.
