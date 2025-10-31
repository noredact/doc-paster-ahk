## DoctorPaster (beta.1)

DoctorPaster is a small AutoHotkey v2 GUI utility for loading a text/CSV file and quickly pasting selected entries using the numeric keypad. It provides a directory viewer, a 9-element preview/paste window, jump controls, a minimal tooltip (compact) mode, and a few user-configurable options.

Important: download the entire repository before running the script
- Use the repository web UI's "Code → Download ZIP" button or `git clone` to download the whole project. Many features expect supporting files to be present in `src/` and `src/default-load-directory/` (for example `src/icon.ico` and the default `replace-me.txt`). If you only copy the `.ahk` script without the `src` folder and its files the program may not behave as expected.

This repository contains the script `doctorPaster.beta.1.ahk` which requires AutoHotkey v2 (not v1).

## Quick summary
- Loads a text/CSV file and shows 9 consecutive elements at a time.
- Use the Numpad keys to paste items or navigate.
- Offers preview panels, directory browsing, adjustable font/transparency, and a minimal tooltip mode for quick one-click pasting.

## Requirements

- Windows (script was developed and tested on Windows).
- AutoHotkey v2+ (the script contains `#Requires AutoHotkey v2+`).

Note: AutoHotkey v1 (classic) is not compatible with this script.

## Installing AutoHotkey v2

1. In your browser open https://www.autohotkey.com/.
2. Click the download link for AutoHotkey v2 (look for "v2" or "Latest v2").
3. Double-click the downloaded installer and follow the prompts.

After installation, Windows should associate `.ahk` files with AutoHotkey so you can run scripts by double-clicking them in File Explorer.

## Running the script

1. Download the whole repository and extract it to a folder you control (for example: `C:\Users\YourName\Documents\DoctorPaster`).
2. Ensure the `src` folder and its contents (notably `src/icon.ico` and `src/default-load-directory/replace-me.txt`) are present.
3. Double-click `doctorPaster.beta.1.ahk` in File Explorer to run it. You can also right-click and choose "Run Script".

Notes:
- If double-clicking doesn't run the script, verify AutoHotkey v2 is installed and that `.ahk` files are associated. You can also right-click and use "Open with" → AutoHotkey.
- If you need an .exe to run on a PC without AutoHotkey installed, you can optionally use the AutoHotkey compiler (AHK2Exe) to convert the script to an executable. See AutoHotkey docs for details.

## Files to keep in the same folder (important)
- `doctorPaster.beta.1.ahk` — the main script (run this).
- `src/icon.ico` — optional icon used by the tray icon when running uncompiled.
- `src/default-load-directory/replace-me.txt` — default sample file the script can load on first run.

If you move the script, keep the `src` folder next to it or update paths inside the script accordingly.

## Quick-start (super simple)

1. Double-click `doctorPaster.beta.1.ahk` to start the GUI.
2. Use the file picker or press `Ctrl+O` to open a text/CSV file.
3. Use Numpad 1–9 to paste items shown in the 9-element preview (ensure NumLock is enabled).


## Troubleshooting

- Nothing happens when pressing Numpad keys: Ensure NumLock is enabled and the script is running. Some laptops require "Fn" or an external numeric keypad to generate Numpad keys.
- Paste not working: The script copies the selected element to the clipboard and sends Ctrl+V. Ensure the target application accepts Ctrl+V and that both the script and target app run at the same privilege level.
- File fails to load: Use the "Change Directory" button in the GUI or `Ctrl+O` to pick a valid text/CSV file. The directory view lists files in the parent directory of the loaded file.

## Contributing

1. Fork the repository.
2. Create a branch for your changes.
3. Submit a pull request with a clear description and testing notes.

If you add hotkeys or change behavior, update this README accordingly.

## License

This project is provided under the MIT License. See the included `LICENSE` file for full terms.

## Contact / Feedback

Open an issue with steps to reproduce and any relevant files.

---


