![image](https://github.com/user-attachments/assets/0247f0fd-da42-4f7a-87b8-a7f49783ac70)

# My PyScript Local Runtime Project

This is my personal offline PyScript setup project. It includes a Python script to download all required PyScript and Pyodide runtime files into a local folder.

---

## 🔧 Steps to Run `setup.py`

1. Open terminal or command prompt.
2. Navigate to the `runtime` folder:

```bash
cd runtime
Run the setup script:

bash
Always show details

Copy
python setup.py
Wait for the downloads to complete. Check setup.log for any errors.

📁 Folder Structure

Always show details

Copy
pyscript-local-runtime/
│
├── runtime/
│   ├── setup.py           # Downloads runtime files
│   ├── setup.log          # Download log
│   ├── [downloaded files] # Includes .js, .whl, .tar, .wasm, etc.
│
├── index.html             # Main PyScript UI
├── main.py                # Optional logic
├── manifest.json          # For Chrome Extension
├── popup.png              # Extension icon
└── README.md              # This file
✅ All files needed to run PyScript locally are downloaded by setup.py.
