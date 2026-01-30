# Focus-Pulse-Web-Dev-Project-
Focus Pulse is a lightweight browser-based focus tracker that measures real study time, detects tab-switch distractions and inactivity, and generates a focus score. Built with HTML, CSS, and Vanilla JavaScript, it runs fully client-side using browser APIs and localStorage for privacy-first insights.
The entire application runs fully in the browser using standard web technologies. There is no backend, no authentication, no browser extensions, and no external data storage. All session data is stored locally using the browser’s localStorage, ensuring complete privacy and offline usability.

🎯 Problem Statement

Students often plan to study for a fixed duration, but distractions like tab switching, background inactivity, or multitasking silently reduce real focus time. Focus Pulse makes these invisible habits visible by tracking focused time, idle time, and distractions in real time, helping users build better study awareness and consistency.

⚙️ Key Features

> Create focus sessions with a task name, duration, and inactivity threshold

> Real-time countdown timer with drift correction using Date.now

> Automatic detection of distractions when the browser tab becomes hidden

> Inactivity tracking using keyboard and mouse events

> Live session status indicator (Focused / Idle / Hidden)

> Focus score (0–100) calculated based on focused time, idle time, and distractions

> Session summary displayed after completion

> Persistent session history stored in localStorage

> Aggregate insights such as total focus time and average focus score

> Optional visualization of session data

> Fully responsive and accessible UI

🧠 How It Works

When a session starts, the app creates a session object and begins tracking time accurately using timestamps rather than relying solely on browser timers. User activity is continuously monitored, and inactivity is detected if no keyboard or mouse interaction occurs for a specified duration. Tab switches are detected using the browser’s visibility API and logged as distractions.

At the end of the session, the app computes focused time, idle time, distraction count, and a final focus score. All completed sessions are saved locally and displayed in a history view for review and self-analysis.

If the page reloads during an active session, the app automatically restores the session from local storage and continues tracking without data loss.

🛠️ Tech Stack

> HTML5 (semantic structure)

> CSS3 (responsive and accessible design)

> Vanilla JavaScript (ES6)

Browser APIs:

> document.visibilitychange

> Keyboard and mouse event listeners

> localStorage

> Date.now for accurate timing

Optional: Chart.js for data visualization

🔐 Privacy & Performance

> No backend or server communication

> No user accounts or tracking

> All data stays on the user’s device

> Optimized to handle hundreds of sessions smoothly

> Timer drift kept under one second for long sessions

📱 Accessibility & Responsiveness

The interface is designed to be minimal and distraction-free, with:

> Semantic HTML elements

> Keyboard-operable controls

> Visible focus states

> Clear status indicators

> Mobile-friendly layout starting from small screen widths
