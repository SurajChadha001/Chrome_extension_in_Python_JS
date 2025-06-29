
```markdown
# My PyScript Local Runtime Project (Personal Use)

This is my personal project to run PyScript locally by downloading all the required Pyodide and PyScript files. It also includes an HTML file and optional Chrome extension setup with popup UI.

---

## ✅ What I Did

- Created a Python script `setup.py` to download all required files from the internet.
- Saved them inside the `runtime/` folder.
- Added an `index.html` to use PyScript locally.
- Included `manifest.json` and `popup.png` in case I want to test this as a Chrome Extension.

---

## 📁 Folder Overview

```

pyscript-local-runtime/
│
├── runtime/
│   ├── setup.py          # Downloads PyScript and Pyodide files
│   ├── setup.log         # Logs success or errors from the download
│   ├── \[downloaded JS/WASM/WHL files]
│
├── index.html            # Main PyScript HTML interface
├── main.py               # PyScript Python code (optional)
├── finished.js           # JS logic (optional, for after loading)
├── manifest.json         # For Chrome extension (optional)
├── popup.png             # Icon for extension popup
└── README.md             # This file (for me)

````

---

## 🔧 How I Run It

### 1. Download Runtime Files

I open a terminal and run:

```bash
cd runtime
python setup.py
````

This creates or updates the downloaded files and logs everything in `setup.log`.

---

### 2. View My App

I open `index.html` in the browser, or right-click it in VS Code and use **Live Server**.

---

### 3. Test Chrome Extension (Optional)

If I want to load this as a browser extension:

* Go to `chrome://extensions/`
* Turn on "Developer Mode"
* Click “Load unpacked”
* Choose the root project folder

It shows a popup using the `popup.png` icon and can load the HTML.

---

## 💬 Notes 

* If anything fails, check `setup.log` in the `runtime/` folder.
* I can add more `.whl` or `.tar` packages to download by editing the `downloads` list in `setup.py`.
* If I update the version of Pyodide or PyScript, I must change the URLs in `setup.py`.

---

## ✅ Status

Everything works locally. Setup script runs without error, files are downloaded, and PyScript loads fine in `index.html`.

