# 🎧 Audio Script

**Audio Script** is a simple browser-based tool for recording segmented audio from a script and merging everything into a single file.

It was built as part of a challenge:

> *"Can AI replace a developer for this kind of tool?"*

Short answer: apparently… yes. Long answer: also yes, but with style.

---

## 🚀 Features

* ✂️ Split your script into multiple recording segments
* 🎙️ Record each segment individually
* 🔁 Re-record any segment with a single button
* 🧠 Automatic project loading (no manual load needed)
* 💾 Save everything locally using `localStorage`
* 🧹 Clear all saved data instantly
* 🧩 Support for inline comments using `//`

  * These appear as visual notes (not audio)
* 🔊 Merge all recordings into a single `.wav` file
* ⏱️ Optional gap between segments

---

## 🧠 How to Use

1. Paste your script into the text box
2. Use `//` to add comments or directions:

   ```
   Line 1
   Line 2
   // pause here
   Line 3
   ```
3. Click **Split**
4. Record each segment
5. Click **Generate final audio**
6. Download your file

---

## 💾 Saving System

* Projects are stored in your browser using `localStorage`
* When you reopen the page, everything loads automatically
* No backend, no accounts, no tracking

---

## ⚠️ Clear Button

The **Clear** button:

* Deletes all saved data
* Reloads the page

There is no undo.
There is only regret.

---

## 🧱 Tech Stack

* HTML
* CSS
* JavaScript (Vanilla)
* Web Audio API
* MediaRecorder API

No frameworks. No dependencies. Just raw browser power and questionable decisions.

---

## 🌍 Live Version

👉 https://audioscript.vercel.app/

---

## 📦 Project Repository

👉 https://github.com/jhonny1307/audioscript

---

## 🧩 Why This Exists

This project was inspired by a simple idea:

> Take a Python tool
> Rebuild it using only AI assistance
> Improve it along the way

Somewhere between curiosity and chaos, this came out.

---

## 🤖 Credits

Made with the help of **ChatGPT** (help like this... slave labo-)

---

## 📜 License

Do whatever you want with it.
Seriously.
