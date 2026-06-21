<div align="center">

```
       _       _                                       _
   ___(_)_ __ | |__   ___ _ __    ___ ___  _ __  ___  ___ | | ___
  / __| | '_ \| '_ \ / _ \ '__|  / __/ _ \| '_ \/ __|/ _ \| |/ _ \
 | (__| | |_) | | | |  __/ |    | (_| (_) | | | \__ \ (_) | |  __/
  \___|_| .__/|_| |_|\___|_|     \___\___/|_| |_|___/\___/|_|\___|
        |_|
```

### `cipher.console`

**A zero-egress operator toolkit for hashing, encryption, encoding, file analysis & search reconnaissance.**

Everything runs in your browser. No backend. No telemetry. No data ever leaves your machine.

<br>

[![Live Demo](https://img.shields.io/badge/live-demo-a3e635?style=for-the-badge&logo=githubpages&logoColor=070907)](https://SRJTools.github.io/SRJConsole/)
[![License: MIT](https://img.shields.io/badge/license-MIT-4dd0c9?style=for-the-badge)](LICENSE)
[![Made with Vanilla JS](https://img.shields.io/badge/vanilla-JS-ffb13b?style=for-the-badge&logo=javascript&logoColor=070907)](#)

![HTML5](https://img.shields.io/badge/HTML5-1c241c?style=flat-square&logo=html5&logoColor=a3e635)
![CSS3](https://img.shields.io/badge/CSS3-1c241c?style=flat-square&logo=css3&logoColor=a3e635)
![No Build Step](https://img.shields.io/badge/build-none-1c241c?style=flat-square)
![Dependencies](https://img.shields.io/badge/runtime%20deps-1%20(CDN)-1c241c?style=flat-square)
![Offline Capable](https://img.shields.io/badge/client-side-1c241c?style=flat-square)

</div>

---

## ◢ Overview

`cipher.console` is a single-file, static security toolkit built for analysts who live in the terminal. It bundles 15 day-to-day operator tools behind a CRT-phosphor interface — fast to load, fully offline-capable, and deployable anywhere a static file can sit.

No accounts. No servers. No "send to API." Open the page and work.

```
┌─ zero egress ──────────────────────────────────────────┐
│  All cryptographic operations execute locally in the    │
│  browser via the Web Crypto API and CryptoJS. Inputs,   │
│  files, and outputs never touch a network.              │
└─────────────────────────────────────────────────────────┘
```

## ◢ Features

### Transform
| Tool | Description |
|------|-------------|
| **hash** | MD5, SHA-1, SHA-256, SHA-512 & SHA3-256 digests computed simultaneously |
| **aes cipher** | AES-256-CBC encrypt / decrypt with random key + IV generation |
| **hmac** | Keyed message authentication — SHA-256/512, SHA-1, MD5 |
| **jwt decode** | Split & decode header / payload, with expiry validation |

### Encode
| Tool | Description |
|------|-------------|
| **base64** | Unicode-safe encode / decode |
| **url** | Percent-encoding codec |
| **hex** | Text ⇄ hexadecimal byte conversion |
| **caesar** | Classic rotation cipher with adjustable shift |
| **vigenère** | Keyword-driven polyalphabetic cipher |

### Generate
| Tool | Description |
|------|-------------|
| **password** | High-entropy secrets via `crypto.getRandomValues`, with live strength meter |
| **uuid · bytes** | UUIDv4 minting + random hex / Base64 byte generation |

### Analyze
| Tool | Description |
|------|-------------|
| **file inspect** | Local fingerprinting: MD5/SHA-256, magic-byte type detection, size, Shannon entropy |
| **network** | IPv4 subnet calculator — network, broadcast, usable range & host count from CIDR/netmask |
| **ioc extract** | Pull URLs, IPv4s, emails & hashes from raw text — with automatic re-fanging |
| **dork engine** | 87 categorized Google dorks with risk filtering, search & one-click launch |

## ◢ Highlights

- **⌘K / Ctrl+K command palette** — fuzzy-jump to any tool instantly
- **Click-to-copy** — every output line copies on click
- **Boot sequence** — animated cold-start, because aesthetics matter
- **Toast notifications** — non-blocking feedback on every action
- **Fully responsive** — collapses cleanly to mobile
- **Respects `prefers-reduced-motion`** — all animation is opt-out
- **Printable CV mode** — `whoami` section exports to clean PDF

## ◢ Tech Stack

```
HTML5  ·  CSS3 (custom properties, grid)  ·  Vanilla JavaScript (ES6+)
CryptoJS 4.1.1 (CDN)  ·  Web Crypto API  ·  Google Fonts (Space Grotesk · JetBrains Mono)
```

No framework. No bundler. No `node_modules`. Just one `index.html`.

## ◢ Run Locally

Because it's a static file, there's nothing to build:

```bash
# clone
git clone https://github.com/SRJtools/SRJConsole.git
cd cipher-console

# open directly...
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows

# ...or serve it
python3 -m http.server 8000
# → http://localhost:8000
```

## ◢ Deploy to GitHub Pages

```bash
# from the repo's Settings → Pages:
#   Source:  Deploy from a branch
#   Branch:  main  /  (root)
#   Save
```

Live within ~1 minute at `https://SRJTools.github.io/SRJConsole/`.

## ◢ Disclaimer

> The **dork engine** is provided for authorized security testing, research, and educational purposes only. Always operate within the bounds of the law and only against assets you own or are explicitly permitted to test. The author assumes no liability for misuse.

The cipher tools (Caesar, Vigenère) are included for educational and CTF use — they are **not** cryptographically secure and must never be used to protect real data.

## ◢ License

Released under the [MIT License](LICENSE). Free to use, modify, and distribute.

---

<div align="center">

**Built by [Sohaib Jad Allah](https://www.linkedin.com/in/sohaibjadallah)**

Security Analyst · DFIR · Jordan

[![LinkedIn](https://img.shields.io/badge/LinkedIn-1c241c?style=flat-square&logo=linkedin&logoColor=a3e635)](https://www.linkedin.com/in/sohaibjadallah)
[![GitHub](https://img.shields.io/badge/GitHub-1c241c?style=flat-square&logo=github&logoColor=a3e635)](https://github.com/SohaibJadAllah)

<sub>`operator@cipher:~$` — built local, runs local.</sub>

</div>
