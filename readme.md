<p align="right">
  <a href="https://buymeacoffee.com/hashcomparator" target="_blank" rel="noopener noreferrer">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" height="36">
  </a>
</p>

<h1 align="center">Hash Compare & Queue</h1>

<p align="center">
  <img src="docs/logo.png" alt="Hash Compare & Queue logo" width="240"/>
</p>

<p align="center">
  <a href="https://github.com/liamdou/Hash-Compare-Queue/releases/latest">
    <img src="https://img.shields.io/badge/⬇%EF%B8%8F%20Download-Latest%20Release-2ea44f?logo=github" alt="Download latest release">
  </a>
</p>

<p align="center">
  🪟 Windows · 🍎 macOS · 🐧 Linux
</p>

---

## ℹ️ About — What is this program?

**Hash Compare & Queue** (HCQ) is a hashing, comparing and more importantly queueing program (yes, I know, duh) for validating that two sets of files are identical and non-corrupt. I made this because I video edit and do A LOT of backing up said videos, on a Mac, which is a much less free platform, where everyone wants to charge for any amount of polish. More importantly, I've never seen a program on any OS (possibly I didn't search hard enough) that allows you to queue up you files to hash compare. Thus this program is born! I wanted to keep it free because that's precisely why I made it in the first place - I couldn't find a free program that does this - so it seems a little hypocritical to charge for it. I'll take [donations](https://buymeacoffee.com/hashcomparator) though if you want to buy me a coffee or a meal ;) Or not, if you don't feel like it :)

## ☕ Use case

Normally, you start up comparing 10 files, you get up to get a coffee or go to the bathroom and you come back, you have to wait until the existing operation is done before you can add more files. With HCQ, you can add 10 files, get up, come back and attach another drive, add 35 more files, find even more files, and add another 105 files to the queue, and it will just keep chugging along.

---

## 🔮 Future

I consider this app pretty feature complete at present. This is as robust if not more than I personally needed it to be. It's gone from MVP (minimum viable product) with my own criteria & requirements to adding a few feature enhancements.

I may fix a couple things like the progress bar's percentage being hard to read on systems with light mode, but any future features/enhancements may be a paid "pro" app, but just something like $5, nothing crazy. I already have a few ideas for what people might ask for but that I personally do not need. I think going beyond features that I initially needed and was looking for, and adding features I personally do not need for other people is a justifiable reason for charging for a coffee. I'll just have to figure out how the logistics of setting that up works.

---

## ✨ Features

- 📂 **Browse** or 🖱️ **Drag & Drop** files or folders for easy folder selection  
- 🔗 **Auto-pair by filename** when **queueing** jobs  
- 🚦 **Threaded** UI elements (NOT hashing) for responsive UI  
- 📏 **Early size check** (skip hashing if sizes differ)  
- ⏹️ **Abort** mid-run (per row or global)  
- ⌫ **Delete** to remove selected queued jobs  
- ⏳ **Live progress** with percent overlay and counts  
- 🧾 **System Message** panel for actions & statuses  
- 🙈 **Ignore `._` files** option (macOS AppleDouble)
- ⚠️ **Error-handling** error messages when there are no matching files, no files selected, etc

---

## 🐞 Issues?

1. You do have to for your first queued batch  press queue first before the compare button. It took too long to just figure out how to automatically detect that just for the first queue vs also detecting when it's not the first queue and ignore it if you press it again. The rest of the queue after you started you can just press Queue and it'll add to the queue and auto-start.
2. You do have to press queue EACH TIME you add a batch of files to Set A/B, because the next batch you drag and drop or browse will erase the existing in Set A/B box. If you drag and drop three different times THEN press Queue, it'll only queue up the latest batch.

Spotted a bug or want a feature? Please open an **Issue** with:  
- 💻 OS (Windows/macOS/Linux) & version  
- 🏷️ App version (release tag)  
- 🔁 Steps to reproduce  
- 🧩 Relevant snippet from **System Messages** (if any)  
*(Please avoid sharing proprietary files.)*

---

## 🖼️ Showcase

**✅❌ Results — Match**
![Match screenshot](docs/screenshots/match.png)
**🧺 Queue**
![Queue screenshot](docs/screenshots/queue.png)
---

## 📦 Installation

**Portable app — no installer.**

Simply download🧳 the archive for your OS from **Releases**. Unzip it and keep the _internal folder and the executable together and run the executable (Mac version doesn't have an _internal folder). The _internal folder contains dependancies the app needs.

---

## 🗑️ Uninstallation

Just **delete the folder** containing the app and the _internal folder.

---

## 🚀 Getting Started

1. ➕ Add files/folders to **Set A** and **Set B** using **Browse** or **drag & drop**.  
2. 🙈 (Optional) Enable **“Ignore files starting with '._'”** when comparing macOS directories.  
3. 🧮 Click **Queue Job** to auto-pair files (by **matching filename** across both sets.)  
4. ⌫ (Optional) Review **Queued Jobs** to remove any mistaken selections (select row → **Delete/Backspace**).  
5. ⚙️ Click **Compare Hashes** to start.
6. 🧺 For additional queues you can just press repeat 1 & 3 (drop / drop files then press queue) without pressing the compare button, they will be auto-started.
7. 👀 Watch **progress** & **System Messages**.  
8. 🟢 Results appear in **Hashes** as:  
   - **✅ Match** – hashes identical  
   - **❌ Mismatch** – hashes differ  
   - **📏 Size mismatch** – sizes differ (hashing skipped)  
   - **🛑 Aborted** / **⚠️ Error**  

---

## 📜 License

License: Proprietary Freeware (PFL). Free for personal/educational/internal evaluation.
Redistribution, modification, reverse-engineering, and commercial use are not permitted.
Please share via the official release link rather than passing files.
For commercial licensing, contact hashcomparator@gmail.com
© 2025 liamdou
