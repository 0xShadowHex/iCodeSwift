<div align="center">

<img src="https://icodeswift.pages.dev/resources/icodeswift_banner.png" alt="iCodeSwift Banner" width="100%" />

<br />

# iCodeSwift

**Run Swift in your browser — no Xcode, no Mac required.**

[![Deployed on Cloudflare Pages](https://img.shields.io/badge/Deployed%20on-Cloudflare%20Pages-F38020?logo=cloudflare&logoColor=white)](https://icodeswift.pages.dev)
[![Swift Toolchain](https://img.shields.io/badge/Swift-5.8-FA7343?logo=swift&logoColor=white)](https://swift.org)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Made by](https://img.shields.io/badge/Made%20by-0xShadowHex-black?logo=github)](https://github.com/0xShadowHex)

[**Live Demo →**](https://icodeswift.pages.dev)

</div>

---

## What is iCodeSwift?

iCodeSwift is a browser-based Swift playground that lets you write, build, and debug Swift code entirely in your browser — powered by region-optimized VPS instances and a custom Monaco editor integration. No Apple Silicon required.

Whether you're learning Swift, prototyping logic, or just want to test a snippet without firing up Xcode, iCodeSwift has you covered.

---

## Features

| Feature | Description |
|---|---|
| ⚡ **Fast Builds** | Region-optimized VPS instances spin up Swift builds quickly |
| 🖥️ **Monaco Editor** | Full-featured code editor with Swift syntax highlighting |
| 📋 **Live Console** | Streams native Swift build output and runtime logs in real time |
| 🔒 **Secure & Private** | Zero vulnerabilities on vuln tests; only your source files are sent to the build server |
| 💾 **LocalStorage** | Projects are persisted locally in your browser — no account needed |
| ✨ **Beautiful UI** | Smooth animations and a clean, minimal interface |
| 🚀 **No Login** | Click "Get Started" and code immediately |

---

## Getting Started

**Three steps and you're running Swift in the browser:**

```
1. Visit https://icodeswift.pages.dev
2. Click "Get Started" to initialize a new project
3. Write Swift — build, run, and debug with the live console
```

No installation. No account. No Mac.

---

## What You Can Build

### ✅ Supported
- Console applications
- Swift logic and algorithms
- Data structures and standard library exploration
- Swift 5.8 language features and syntax testing
- Learning and experimentation

### ❌ Not Supported
- GUI / SwiftUI apps (VPS environment restriction)
- Downloading compiled Swift binaries (privacy & security constraint)
- Networking or system-level APIs

---

## Tech Stack

- **Frontend** — Vanilla HTML/CSS/JS with custom Monaco Editor integration
- **Hosting** — [Cloudflare Pages](https://pages.cloudflare.com) (fully static frontend)
- **Build Backend** — Region-optimized VPS running the Swift 5.8 toolchain
- **Storage** — `localStorage` for client-side project persistence
- **Editor** — [Monaco Editor](https://microsoft.github.io/monaco-editor/) (the engine behind VS Code)

---

## Architecture Overview

```
Browser (icodeswift.pages.dev)
│
├── Monaco Editor Instance        ← User writes Swift code
├── localStorage                  ← Project state persisted client-side
│
└── Build Request (HTTPS POST)
        │
        └── Region-Optimized VPS
                ├── Swift 5.8 Toolchain
                ├── Build & Execute
                └── Stream stdout/stderr back to console
```

The frontend is fully static and deployed to Cloudflare Pages — no backend, no auth server, no database. The only server-side component is the Swift build VPS.

---

## Project Structure

```
icodeswift/
├── index.html          # Landing page
├── resources/
│   ├── icodeswift_banner.png
│   └── orange_swift_icon.png
├── editor/             # Monaco editor integration & build logic
└── styles/             # UI and animation styles
```

---

## Related Projects

- [**iCodeWin**](https://icodeswift.pages.dev) — A companion project focused on iOS development tooling, built earlier and coded largely from scratch. One of the foundational projects in this series.

---

## Roadmap

- [ ] Multi-file project support
- [ ] Shareable snippet links
- [ ] Swift Package Manager (SPM) dependency support (experimental)
- [ ] Swift 5.9 / 6.0 toolchain support
- [ ] Dark/light theme toggle
- [ ] Syntax error underlining via Language Server Protocol (LSP)

---

## Contributing

Contributions, issues, and feature requests are welcome. If you find a bug or have an idea, open an issue or submit a PR.

```bash
# Clone the repo
git clone https://github.com/0xShadowHex/icodeswift.git

# Open locally — it's a static site, no build step needed
cd icodeswift
open index.html
```

---

## Security

iCodeSwift has been tested and shows **zero vulnerabilities** in standard security audits. Your source code is the only data transmitted to the build server. No telemetry, no tracking, no accounts.

If you discover a security issue, please report it responsibly via [GitHub Issues](https://github.com/0xShadowHex/icodeswift/issues) or direct message.

---

## License

MIT © [0xShadowHex](https://github.com/0xShadowHex)

---

<div align="center">

Built with passion and creativity · [icodeswift.pages.dev](https://icodeswift.pages.dev)

<img src="https://icodeswift.pages.dev/resources/orange_swift_icon.png" alt="Swift Icon" width="48" />

</div>
