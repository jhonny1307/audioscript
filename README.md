# 🎧 Audio Script

**Audio Script** is a lightweight browser-based tool for recording, organizing, previewing, and generating segmented audio from a script.

It started as a challenge:

> *"Can AI replace a developer for this kind of tool?"*

Short answer: yes.  
Long answer: yes… and it kept getting better.

---

## 🚀 Features

* ✂️ Split your script into multiple segments
* 🎙️ Record each segment individually
* 🔁 Re-record any segment instantly
* ⏹️ Stop or interrupt recordings safely
* 📂 Upload external audio files (mp3, wav, etc.)
* ❤️ Toggle favorite segments (include/exclude in preview/export)
* 🎧 Real-time preview of selected segments
* 📥 Download individual audio tracks
* 📦 Export selected tracks as a ZIP
* 📦 Export all tracks as a ZIP
* 🔊 Merge selected segments into a single `.wav` file
* 🔀 Export all segments into a single `.wav` file
* ⏱️ Configurable gap between segments for merged audio
* 🧠 Automatic saving (no save button needed)
* 💾 Persistent storage using `localStorage`
* 🧹 One-click project reset
* 🧩 Inline comments using `//`
  * Displayed as visual notes (not audio)
* 📱 Mobile-friendly interactions (including vibration feedback)
* 🎨 Clean UI with improved readability and structure
* 📌 Floating preview player (always visible)
* 🔄 Manual preview refresh
* 🎛️ Unified export menu with four export options

---

## 🧠 How to Use

1. Paste your script into the text box
2. Add comments using `//` when needed:

```text
Line 1
Line 2
// pause here
Line 3
```

3. Click **Split**
4. Record or upload audio for each segment
5. Optionally mark preferred segments using the toggle
6. Use the **Preview** player to listen before exporting
7. Click **Export** to choose between:
   - **Export Selected Audio** — merges only marked segments into one `.wav`
   - **Export All Audio** — merges all available segments into one `.wav`
   - **Export Selected ZIP** — exports marked segments individually inside a `.zip`
   - **Export All ZIP** — exports all segments individually inside a `.zip`
8. Individual tracks can also be downloaded separately

### 🎧 Preview vs Export

The **Preview** player uses the selected segments and applies the configured gap between them.

The merged audio exports use the same gap configuration.

ZIP exports are different: each segment remains a separate audio file, so there is **no gap added between tracks**.

---

## 💾 Saving System

* Everything is saved automatically
* Uses browser `localStorage`
* No accounts, no backend, no tracking
* Reopening the page restores your project instantly
* Recorded audio is normalized when necessary to ensure reliable duration information

---

## ⚠️ Clear Button

The **Clear** button:

* Deletes all saved data
* Reloads the page instantly

There is no undo.  
There is only regret.

---

## 🧱 Tech Stack

* HTML
* CSS
* JavaScript (Vanilla)
* Web Audio API
* MediaRecorder API
* JSZip

No frameworks. No unnecessary dependencies. No excuses.

---

## 🌍 Live Version

👉 https://audioscript-web.vercel.app/

---

## 📦 Project Repository

👉 https://github.com/jhonny1307/audioscript-web

---

## 🧩 Why This Exists

This project came from a simple experiment:

> Take an existing idea  
> Rebuild it using AI  
> Keep improving it until it stops being simple

Somewhere between curiosity and chaos… this happened.

---

## 🤖 Credits

Built with the help of [**ChatGPT**](https://chatgpt.com/share/69efb636-ea20-83e9-b798-548f8353fe56)

---

## 📜 License

Do whatever you want with it.  
Seriously... or no... or yes...

---

## 📌 Latest Update - V12.1.5

**Date:** `20/08/2026`

| ➕ Added | 🔧 Modified | 🐛 Fixed |
|---|---|---|
| ZIP export for selected tracks<br>ZIP export for all tracks<br>Unified export menu | Preview/export layout redesigned<br>Export menu moved inside the floating Preview panel<br>Manual preview refresh retained<br>Recorded audio normalized to WAV when necessary | Incorrect duration displayed by recorded audio players<br>Export menu positioning and Preview panel layout |

### Export System

The export system now provides four options:

1. **Selected Audio** — merged `.wav` containing only selected tracks
2. **All Audio** — merged `.wav` containing all tracks
3. **Selected ZIP** — ZIP containing selected tracks as individual audio files
4. **All ZIP** — ZIP containing all tracks as individual audio files

Merged exports respect the configured gap between tracks.

ZIP exports contain the original tracks separately and do not add artificial delays between them.
