<div align="center">

# ExCodes.

**A Full Local-First IDE, Isolated Sandbox, AES-256 Vault, QA Lab & AI Agent — Packed Into One Single HTML File.**

*Zero servers. Zero dependencies. Zero subscriptions.*

[![Live Demo](https://shields.io)](https://github.io)
[![Architecture](https://shields.io)](#)
[![License: MIT](https://shields.io)](LICENSE)

[**🚀 Open Live App (`t1rbo.github.io/ExCodes`)**](https://github.io)

</div>

---

## 📖 What is ExCodes?

**ExCodes** is a completely autonomous, zero-dependency development environment built inside a single standalone `index.html` file (~60 KB). 

There is no backend, no build step, no `node_modules`, and no tracking. You can use it online via GitHub Pages or save the single HTML file to your computer/USB drive and code completely offline anywhere.

### 🤝 How It Was Built (Human + AI Synergy)
ExCodes is a real-world experiment in AI-driven software engineering:
- **Concept, Architecture, Testing & Debugging — [t1rbo](https://github.com):** Designed the product vision, combined multiple prototypes, hunted down edge-case parser and UI bugs, and tested every single feature.
- **Core Code Generation — Qwen:** Generated the vanilla JS virtual file system, custom CRC32 ZIP archiver, WebCrypto AES-256-GCM encryption module, and syntax highlighter under strict human guidance.

---

## ✨ Core Features

- **🌐 11 Languages Out of the Box**
  Instant starter repositories (`src/`, `tests/`, `README.md`, `.gitignore`) with custom SVG icons and real-time syntax highlighting for **Python, JavaScript, C++, C, C#, Java, Go, Rust, R, SQL, and Visual Basic**.
- **⚡ Isolated Web Worker Sandbox**
  Run JavaScript safely in a background Web Worker with execution timeout protection, or preview live HTML/CSS/JS projects inside a sandboxed `iframe`.
- **🔐 Zero-Knowledge Vault (`AES-256-GCM`)**
  Client-side encryption powered by native WebCrypto (`PBKDF2` with 310,000 iterations + `AES-256-GCM`) and a 12-word recovery seed phrase. Export and import encrypted `.excodes` workspace snapshots.
- **🧠 Local AI Agent (Ollama Bridge)**
  Connects directly to your local **Ollama** server (`gemma4`, `qwen2.5-coder`, `llama3`, etc.) with visual `diff` previews before applying any file changes. Includes a built-in offline demo agent.
- **🧪 Built-in QA Lab**
  48 automated self-tests verifying the Virtual File System, 50-step undo history, ZIP packer, cryptography, and sandbox runtime.
- **📦 Native Zero-Dependency ZIP & Self-Export**
  Builds valid `.zip` archives from scratch with real CRC32 checksums, plus supports exporting your entire project inside a standalone HTML file.

---

## 🧠 Quick Start: Connecting Local AI (Ollama)

To power the **Agent** panel with local LLMs running on your own GPU/CPU, start Ollama with CORS enabled so the browser can talk to `127.0.0.1:11434`:

**Windows (PowerShell):**
```powershell
$env:OLLAMA_ORIGINS="*"; ollama serve
```

**Linux / macOS:**
```bash
OLLAMA_ORIGINS="*" ollama serve
```

Then open **ExCodes**, click **«Мост» (Bridge)** in the right-hand Agent panel, and choose your installed model (e.g., `gemma4` or `qwen2.5-coder`).

---

## 🛠 Under the Hood

- **100% Pure HTML5, CSS3 & Vanilla JavaScript** (zero frameworks, zero external scripts)
- **WebCrypto API** (`PBKDF2`, `AES-GCM`, `SHA-256`)
- **Web Workers & Blob URLs** for isolated code execution
- **Web Audio API** for synthesized UI sound effects

---

## 💖 Support the Project

If **ExCodes** helped you, saved your time, or inspired you to build local-first tools, feel free to support future updates with a crypto donation:

* **USDT (Network: TRC-20 / TRON):**
  ```text
  TPmnVDCvPSapMRWpbMw2tFS5g1Rw8VJQC1
  ```
* **Bitcoin (BTC — Native SegWit):**
  ```text
  bc1q87gzglw6zyn03w57uyan8r9rudeevcf9w8l8j5
  ```
* **Ethereum (ETH — ERC-20):**
  ```text
  0x129b2C581F21690218B4A6ace2c01eDAACb6eE35
  ```
* **TON / Toncoin (Network: TON):**
  ```text
  UQDiXhQGch21UglmasYRvx9FdC74GKr4fOzETlfzaNzczw0B
  ```

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.
