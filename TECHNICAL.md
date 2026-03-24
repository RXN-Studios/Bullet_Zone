# Technical Logic & Data Management

## 💾 State Persistence
BulletZone utilizes a custom `localStorage` wrapper to ensure player data persists across browser sessions.
* **Save Key:** Uses a unique identifier to prevent collisions with other local applications.
* **Data Structure:** Stores High Scores, Audio preferences (Music/SFX), and unlocked weapon Sets in a JSON-parsed object.

## 🖥️ UI/UX Architecture
The game uses a **State-Based UI** system to manage transitions between the Home Screen and active gameplay:
* **Overlay Management:** Uses CSS classes to transition between menus and the game arena without page reloads.
* **Responsive Layouts:** Designed to scale dynamically from desktop monitors to mobile devices using `clamp` and `min` CSS functions for fluid typography and element sizing.

## 🔊 Audio Engine
* **Independent Channels:** Separate toggles for Music and SFX allow for a customized user experience.
* **Sync Logic:** Audio states are synced across the UI and the local storage to maintain preferences between sessions.
