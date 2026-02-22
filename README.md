# 📁 File Cleaner

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" />
  <img src="https://img.shields.io/badge/Built%20With-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <a href="https://www.buymeacoffee.com/YOUR_USERNAME">
    <img src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black" />
  </a>
</p>

**A sleek, automated desktop file organizer for Windows.** File Cleaner continuously watches your Downloads (or any target folder) and instantly routes files to specific destinations based on rules you create. Unlike basic organizers, it features **Deep Content Scanning**, allowing it to read inside PDFs and Word documents to sort them even if the filename is vague.

## ✨ Features

* **🔍 Deep Content Search:** Reads the actual text inside `.pdf`, `.docx`, and `.txt` files to find keywords for routing.
* **🍎 Minimalist UI:** A clean, modern interface built with `customtkinter`.
* **⚡ Real-Time Monitoring:** Uses `watchdog` to detect and move files the instant they are saved.
* **👻 System Tray Integration:** Runs silently in the background. Double-click the tray icon to wake or sleep the app.
* **🧠 Smart Resume:** Prevents duplicate instances. Opening the app while it's hidden just brings the existing window to the front.
* **📅 Auto-Scan Scheduler:** Set it to clean your folders Daily, Weekly, or Monthly automatically.

## 🚀 How to Download & Run

**No coding required!**
1.  Go to the **[Releases](../../releases)** page on the right sidebar.
2.  Download the latest `FileCleaner.exe`.
3.  Double-click to run. (You might need to tell Windows it's safe to run since it's a new app).

## 🛠️ For Developers (Build from Source)

If you want to tweak the code or build it yourself:

1.  **Clone the repo**
    ```bash
    git clone [https://github.com/3boodMMVI/File-Cleaner.git](https://github.com/3boodMMVI/File-Cleaner.git)
    cd File-Cleaner
    ```

2.  **Install Dependencies**
    ```bash
    pip install customtkinter watchdog pystray schedule pypdf python-docx pillow
    ```

3.  **Run the Script**
    ```bash
    python Main.py
    ```

4.  **Compile to .exe**
    ```bash
    python -m PyInstaller --noconsole --onefile --icon=icon.ico --add-data "icon.ico;." --collect-all customtkinter Main.py
    ```

---

*Enjoying the tool? [Buy me a coffee](https://www.buymeacoffee.com/YOUR_USERNAME) to support future updates!* ☕
