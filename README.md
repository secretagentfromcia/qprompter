<div align="center">
  <img src="extension/icons/icon128.png" width="80" alt="Qprompter Logo">
  <h1>Qprompter</h1>
  <p><strong>Queue your prompts. Automate your AI chat workflows.</strong></p>

  <a href="https://github.com/YOUR_USERNAME/qprompter/releases/latest">
    <img src="https://img.shields.io/github/v/release/YOUR_USERNAME/qprompter?color=0ea5e9&label=Download&style=for-the-badge" alt="Download">
  </a>
  <img src="https://img.shields.io/badge/Manifest-V3-22c55e?style=for-the-badge" alt="MV3">
  <img src="https://img.shields.io/badge/License-MIT-f59e0b?style=for-the-badge" alt="MIT">
  <img src="https://img.shields.io/github/issues/YOUR_USERNAME/qprompter?style=for-the-badge" alt="Issues">
</div>

---

## What is Qprompter?

Qprompter is a free, open-source Chrome extension that lets you build a **queue of prompts** and fire them automatically at any AI chat platform — with smart delays, response detection, and background execution.

Stop copy-pasting. Stop watching the screen. Build your workflow once, press Start, walk away.

---

## ✅ Supported Platforms

| Platform | Status |
|---|---|
| ChatGPT (chatgpt.com) | ✅ Supported |
| Claude (claude.ai) | ✅ Supported |
| Gemini (gemini.google.com) | ✅ Supported |
| Microsoft Copilot | ✅ Supported |
| Poe | ✅ Supported |
| Character.AI | ✅ Supported |
| Bing AI | ✅ Supported |

---

## 🚀 Features

### 📋 Smart Prompt Queue
Build an ordered list of prompts and send them one by one, automatically. Each prompt runs after the previous AI response finishes — no guessing, no overlap.

### ⏱️ Configurable Delays
Set a custom cooldown between each prompt in **seconds or minutes**. The first prompt fires immediately on Start; delays apply from the second onward.

### 🧠 AI Response Detection
Multi-signal engine waits for the AI to *actually finish* before moving to the next prompt. Combines:
- Stop-button and spinner UI detection
- DOM mutation stream analysis
- Background network request tracking (WebRequest API)

### 🔁 Variable Prompt Generator
Write one template with a `{value}` placeholder, supply a comma-separated list of values, and instantly generate 10, 50, or 100 prompt variations queued and ready.

### 🖼️ Image Mode
Tag any prompt as an image generation prompt for proper handling on image-capable models.

### 📁 Bulk TXT Import
Import a `.txt` file where each line becomes a separate queued prompt. Batch-load entire workflows in one click.

### 📚 Template Library
Save and reuse your best prompts with a searchable, categorized library. Comes preloaded with Marketing, Coding, Social Media, and Business templates.

### 📜 History Log
Every sent prompt is logged with timestamp, delay, and status. Re-queue any past prompt with one click.

### 🔔 Webhook Simulator
Simulate external system alerts (GitHub CI failures, Sentry crashes, Stripe disputes) as pre-formatted prompts — ideal for DevOps AI automation workflows.

### 🌐 Background Execution
Runs entirely in the Chrome service worker using the Alarms API. Close the popup — your queue keeps running. Switch tabs. It keeps running.

### 🎨 Light & Dark Theme
Full high-contrast light theme toggle for accessibility.

### 🔒 100% Local & Private
Zero analytics. Zero telemetry. Zero external servers. All data stays in your browser's local storage.

---

## 📦 Installation

Qprompter is not on the Chrome Web Store. It installs in 4 steps via Chrome's built-in Developer Mode — this is safe, standard, and takes under 2 minutes.

### Step-by-Step

**1. Download the extension**
👉 Go to [Releases](https://github.com/YOUR_USERNAME/qprompter/releases/latest) and download `qprompter-vX.X.X.zip`

**2. Unzip the file**
Extract the zip. You should see a folder called `qprompter` containing `manifest.json` and other files.

**3. Open Chrome Extensions**
Navigate to `chrome://extensions` in your browser address bar.

**4. Enable Developer Mode**
Toggle **Developer Mode** ON in the top-right corner.

**5. Load the extension**
Click **"Load unpacked"** → select the unzipped `qprompter` folder → click OK.

That's it. The Qprompter icon appears in your toolbar. 🎉

> **Does this work on Edge?** Yes. Edge supports Chrome extensions and the same load-unpacked process works at `edge://extensions`.
> 
> **Will I get automatic updates?** Not automatically — check the Releases page for new versions. You'll need to replace the folder and reload.

---

## 🎮 How to Use

1. **Open any supported AI chat** (ChatGPT, Claude, Gemini, etc.)
2. **Click the Qprompter icon** in your toolbar
3. **Type or paste prompts** in the composer, set a delay, click **ADD**
4. Optionally import from a `.txt` file or use the Variable Generator
5. Click **START** — the first prompt fires immediately
6. Watch the queue run. Pause or Stop anytime. Close the popup — it keeps going.

---

## 🛠️ Troubleshooting

**Send button not activating after prompt is typed?**
Make sure you're on a supported platform. Some platforms update their UI frequently — [file an issue](https://github.com/YOUR_USERNAME/qprompter/issues/new?template=bug_report.md) with your platform name.

**Queue paused with "No AI tab found"?**
Open an AI chat tab before starting the queue, or disable "Pause if No Tab" in Settings.

**Extension stopped working after Chrome update?**
Go to `chrome://extensions`, find Qprompter, and click the reload button (↻).

---

## 🗺️ Roadmap

- [ ] Firefox support (Manifest V3 compatible)
- [ ] Drag-to-reorder in variable generator
- [ ] Export/import queue as JSON
- [ ] Per-prompt platform targeting
- [ ] Webhook receiver via native messaging

---

## 🤝 Contributing & Feedback

Found a bug? Have an idea? 

- 🐛 [Report a Bug](https://github.com/YOUR_USERNAME/qprompter/issues/new?template=bug_report.md)
- 💡 [Request a Feature](https://github.com/YOUR_USERNAME/qprompter/issues/new?template=feature_request.md)
- 💬 [Join the Discussion](https://github.com/YOUR_USERNAME/qprompter/discussions)

PRs welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## 📄 License

MIT — free to use, modify, and distribute. See [LICENSE](LICENSE).
