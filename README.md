<div align="center">

# ExCodes.

**Local-First IDE, Isolated Sandbox, AES-256 Vault, QA Lab & AI Agent in a Single HTML File.**

*Zero servers. Zero dependencies. Zero subscriptions.*

[![Live Demo](https://shields.io)](https://github.io)
[![Single File](https://shields.io)](#)
[![License: MIT](https://shields.io)](LICENSE)

[**🚀 Launch ExCodes Live**](https://github.io)

</div>

---

## 📖 About the Project

**ExCodes** is an experimental, self-contained browser development environment packed entirely into a single standalone `index.html` file (~60 KB, zero external libraries or build steps). 

You can run it directly on GitHub Pages, download the single HTML file to a USB drive, and code completely offline with built-in encryption, isolated execution, and a local AI assistant.

### 🤖 How It Was Built (Human + AI Synergy)
This project is a showcase of modern AI-assisted software engineering:
- **Architecture, Concept, Testing & Debugging:** **[t1rbo](https://github.com)** — designed the multi-module architecture, merged prototypes, fixed edge-case parser bugs, and tested every component.
- **Core Code Generation:** **Qwen** — generated the zero-dependency VFS engine, custom CRC32 ZIP packer, WebCrypto AES-256-GCM vault, and syntax highlighter under human direction.

---

## ✨ Key Features

- **🌐 11 Languages Out of the Box**
  Instant starter repositories (`src/`, `tests/`, `README.md`, `.gitignore`) with custom SVG icons and syntax highlighting for **Python, JavaScript, C++, C, C#, Java, Go, Rust, R, SQL, and Visual Basic**.
- **⚡ Isolated Web Worker Sandbox**
  Run JavaScript safely inside an isolated Web Worker with execution timeout protection, or preview live HTML/CSS/JS bundles in a sandboxed iframe.
- **🔐 Zero-Knowledge Vault (`AES-256-GCM`)**
  Client-side encryption powered by native WebCrypto (`PBKDF2` with 310,000 iterations + `AES-256-GCM`) and a 12-word recovery seed phrase. Export and import encrypted `.excodes` workspaces.
- **🧠 Local AI Agent (Ollama Bridge)**
  Connects directly to your local **Ollama** instance (`gemma4`, `qwen2.5-coder`, `llama3`, etc.) with visual `diff` previews before applying any changes to your files. Includes an offline demo agent fallback.
- **🧪 Built-in QA Lab**
  48 automated self-tests verifying the Virtual File System, undo stack, ZIP archiver, cryptography, and sandbox environment.
- **📦 Native Zero-Dependency ZIP & Self-Export**
  Generates valid `.zip` archives from scratch with real CRC32 checksums, plus supports exporting your workspace directly inside a standalone HTML file.

---

## 🧠 Connecting Local AI (Ollama)

To use real local LLMs inside the **Agent** panel, start Ollama with CORS enabled so the browser can communicate with `127.0.0.1:11434`:

**Windows (PowerShell):**
```powershell
\$env:OLLAMA_ORIGINS="*"; ollama serve
```

**Linux / macOS:**
```bash
OLLAMA_ORIGINS="*" ollama serve
```

Then click **«Мост» (Bridge)** in the right-hand Agent panel inside ExCodes and select your installed model (e.g., `gemma4` or `qwen2.5-coder`).

---

## 🛠 Tech Stack

- **100% Vanilla HTML5, CSS3 & ES6+ JavaScript** (no React, no Webpack, no npm)
- **WebCrypto API** (`PBKDF2`, `AES-GCM`, `SHA-256`)
- **Web Workers & Blob URLs** for isolated code execution
- **Web Audio API** for synthesized UI sound feedback

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.
