
# My PyScript Local Runtime Project

This is my personal project to set up and run PyScript completely offline using local files. It includes a Python script to download required runtime components and a simple UI that mimics a weather-style extension or single-page app.

---

## ✅ What I Did

- Wrote `setup.py` to download all required PyScript and Pyodide runtime files into the `runtime/` folder.
- Used `index.html` with PyScript to create a local interactive UI.
- Included `manifest.json` and `popup.png` in case I want to test this as a Chrome Extension.
- Verified everything works by checking that files downloaded correctly and UI loads in the browser.

---

## 📁 My Folder Structure

pyscript-local-runtime/
│
├── runtime/
│ ├── setup.py # Downloads runtime files
│ ├── setup.log # Download log
│ ├── pyodide.js, pyodide_py.tar, etc.
│
├── index.html # Main HTML UI (PyScript-based)
├── main.py # Optional PyScript logic
├── finished.js # Optional JS to load after runtime
├── manifest.json # For Chrome Extension
├── popup.png # Icon for popup
└── README.md # This file (for me only)

yaml
Always show details

Copy

---


## 🧪 How I Run Everything

### 1. Download Runtime Files

```bash
cd runtime
python setup.py
This downloads PyScript, Pyodide, and other required assets into the runtime/ folder.

2. Launch the UI
I open index.html in the browser.

Or I use Live Server in VS Code to preview it.

3. (Optional) Test as Chrome Extension
Steps I follow:

Open chrome://extensions/

Enable Developer Mode

Click “Load unpacked”

Select the root project folder

It shows the popup with the icon (popup.png), and loads my UI.

🧾 Notes to Myself
setup.py logs everything in setup.log

If a file fails to download, check the log or internet URL

I can switch Pyodide version by editing URLs in setup.py

I don’t share this project — it’s for my own learning and setup

✅ Everything is working as expected — downloads complete, UI shows properly, and the project runs fully offline after setup.
"""
![image](https://github.com/user-attachments/assets/89d04410-f658-4ab4-85c0-14dcfc542942)


Save to a README.md file
readme_path = Path("/mnt/data/README.md")
readme_path.write_text(readme_content.strip())

