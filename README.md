# 🛰️ P2P Terminal Chat App (Python)

A lightweight, encrypted, peer-to-peer group chat app that runs in the terminal.  
No servers. No cloud. Just raw sockets, AES encryption, and pure Python.

---

## 🚀 Features

- 🌐 **Room-based Chat**: One person hosts, others join via IP:PORT
- 🔐 **End-to-End Encryption**: AES-256 secured messages using a shared room password
- 🧑‍💻 **Nicknames Only**: Peers see only nicknames — host's IP is required, but others stay private
- 🧾 **Local Chat Logs**: Messages saved in `.txt` logs per room
- 🛂 **Moderation**: Host can kick users from the room
- 💻 **Rich Terminal UI**: Clean layout using the `rich` library
- 🛠️ **No Server or Ngrok**: Runs on pure sockets with optional UPnP/port forwarding

---

## 🧰 Tech Stack

- Python 3.x
- `socket`, `threading`, `argparse`
- `pycryptodome` — for AES-256 encryption
- `rich` — for terminal UI
- `miniupnpc` (optional) — for auto port forwarding

---

## 🎮 Demo

![Demo Screenshot](assets/demo.gif)  
_(Optional: Add an asciinema or GIF to show terminal UI in action)_

---

## 📦 Installation

Install via pip:

```bash
pip install p2pchat
