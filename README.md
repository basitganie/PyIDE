# ⚡ PyIDE

![Version](https://img.shields.io/badge/version-1.0.0-cyan)
![License](https://img.shields.io/badge/license-MIT-purple)
![Python](https://img.shields.io/badge/python-3.11-blue)
![Platform](https://img.shields.io/badge/platform-WebAssembly-orange)

**PyIDE** is a sophisticated, browser-based Integrated Development Environment (IDE) designed for seamless Python development. By leveraging WebAssembly, it provides a native-feeling experience with a full virtual file system, multi-module support, and a sleek, modern aesthetic.

---

## 🚀 Key Features

* **Native-Grade Editor:** Powered by **CodeMirror** with JetBrains Mono typography, syntax highlighting, and smart indentation.
* **Virtual File System (VFS):** Create, rename, delete, and organize files and folders within a persistent workspace.
* **Multi-Module Execution:** Unlike basic web-compilers, PyTerminal Pro allows files to import from one another (e.g., `import utils`) by pre-loading the workspace into the Pyodide environment.
* **"Void" UI Design:** A high-contrast, distraction-free interface featuring a dynamic tab system, breadcrumb navigation, and a custom context menu.
* **Scientific Stack:** Out-of-the-box support for `numpy` and other core Python libraries.

---

## 🛠️ Technical Architecture

| Layer | Technology | Description |
| :--- | :--- | :--- |
| **Runtime** | [Pyodide](https://pyodide.org/) | Python 3.11 compiled to WebAssembly (WASM). |
| **Interface** | HTML5 / CSS3 | Custom CSS variables for the "Void" theme and grid-based layout. |
| **Logic** | JavaScript (ES6+) | Custom-built FileSystem class for recursive path resolution. |
| **Editor** | CodeMirror 5 | Industry-standard source code editor for the web. |

---

## ⌨️ Shortcuts & Commands

| Action | Shortcut |
| :--- | :--- |
| **Run Code** | `Ctrl + Enter` |
| **Save File** | `Ctrl + S` |
| **Indent Selection** | `Tab` |
| **Close Tab** | `Click ×` |

---

## 📂 Project Structure

PyTerminal Pro manages a complex virtual directory structure:
```text
/workspace
├── main.py        # Entry point
├── utils.py       # Helper functions
└── examples/      # Folder management
    └── hello.py   # Nested file support


🤝 Contributing
Contributions make the open-source community an amazing place to learn and create.
1. Fork the Project.
2. Create your Feature Branch (git checkout -b feature/AmazingFeature).
3. Commit your Changes (git commit -m 'Add some AmazingFeature').
4. Push to the Branch (git push origin feature/AmazingFeature).
5. Open a Pull Request.
📜 License
Distributed under the MIT License. See LICENSE for more information.
Project Link: https://github.com/basitganie/PyIDE
