✨ M-TOOL — Morrigan Tool

Smart, repo-free Windows driver & runtime installer with a sleek PySide6 GUI.

<p align="center">
  <img src="https://i.imgur.com/scU5KBS.png" alt="M-TOOL logo" width="96" height="96" style="border-radius:14px;" loading="lazy" />
</p>
<p align="center">
  <a href="https://img.shields.io/badge/Platform-Windows_10%2F11-blue?logo=windows&logoColor=white">
    <img src="https://img.shields.io/badge/Platform-Windows_10%2F11-blue?logo=windows&logoColor=white" height="20" />
  </a>
  <a href="https://img.shields.io/badge/GUI-PySide6-7C3AED?logo=qt&logoColor=white">
    <img src="https://img.shields.io/badge/GUI-PySide6-7C3AED?logo=qt&logoColor=white" height="20" />
  </a>
  <a href="https://img.shields.io/badge/Build-PyInstaller%20%7C%20Nuitka-22C55E">
    <img src="https://img.shields.io/badge/Build-PyInstaller%20%7C%20Nuitka-22C55E" height="20" />
  </a>
  <a href="https://img.shields.io/badge/Admin-Required-critical">
    <img src="https://img.shields.io/badge/Admin-Required-critical" height="20" />
  </a>
</p>

⚡ Features

🧠 Auto-detect Motherboard → installs Intel/AMD Chipset + Intel MEI silently (no repo required)
🎮 GPU auto via winget (NVIDIA/AMD/Intel)
🪟 Windows Update (Drivers Only) matched by HWIDs
🧰 Runtimes: .NET 4.7.2 + 4.8, VC++ 2008–2022 (x86/x64)

🧩 What Each Toggle Does

Auto MB Drivers (fast, repo-free) → Intel/AMD chipset + Intel MEI
Vendor Auto (winget) → GPU + common platform bits
Windows Update – Drivers → Installs WHQL drivers matched to your HWIDs
.NET 4.7/4.8 & VC++ 2008–2022 → Silent, idempotent installs

Dry-run → Scan + plan only (no changes)

##🚀 Quick Start (Dev)##
git clone <your-repo>
cd M-TOOL
py -m pip install -r requirements.txt
py mtool_gui.py

🖥️ CLI
# Auto MB only (chipset/MEI)
py -m mtool.cli --auto-mb

# Add runtimes
py -m mtool.cli --auto-mb --vcredist --dotnet

# Add GPU/platform via winget
py -m mtool.cli --auto-mb --vendor-auto

# Use Windows Update (driver only)
py -m mtool.cli --windows-update

📜 License
Add your preferred license (MIT/Apache-2.0) as LICENSE in the repo.

<p align="center">
  Made with ❤️ for clean Windows setups • PRs & issues welcome!
</p>

