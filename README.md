Sure! Here's your content formatted as a professional and clean `README.md` for your GitHub repository:

---

````markdown
# 🛰️ P2PChat — A Peer-to-Peer Encrypted Terminal Chat App

P2PChat is a **fully peer-to-peer, end-to-end encrypted terminal-based chat app** with no servers, no accounts, and no data collection — just raw sockets, passwords, and secure communication.

---

## 🔧 Key Features

- 🧑‍💻 **Host-based Rooms**: One user creates a room and shares an invite code in the format: `IP:PORT#password`
- 🔑 **Join with Invite Code**: Others join the chat room using that invite code
- ☁️ **No Central Server**: No cloud or server dependency — 100% peer-to-peer
- 📮 **Manual IP & Port Entry**: Allows advanced users to connect directly
- 🎓 **.edu Email-Only Rooms** *(future enhancement idea)*
- 🧭 **Host as Lightweight Relay**: Host handles all connections
- 🆔 **Nickname-Only Identity**: IP hidden from peers
- 🔐 **AES Encryption**: Messages encrypted using shared room password
- 📝 **Local Message Logging**: Messages stored locally as `.txt` files
- 🧹 **Kick Support**: Hosts can remove users from room
- 🖥️ **Terminal UI via `rich`**: Colorful, responsive terminal experience
- 🔓 **No Ngrok / Paid Services**: Fully open and local-first
- 🔁 **Optional UPnP Support**: For automatic port forwarding (where available)

---

## 📦 Architecture

> A minimal yet powerful P2P hybrid architecture

- 👤 **Host** acts as the central relay/server for the room
- 🧩 **Peers** connect directly to host via TCP
- 🔐 **AES-256 encryption** with shared room password
- 🗃️ **Local storage** of configs and message history
- ❌ No third-party API or cloud involved

---

## 🔐 Security Model

| Feature           | Description                                           |
|------------------|-------------------------------------------------------|
| 🔒 End-to-end Encryption | Using `pycryptodome` and AES-256                |
| 🕵️ Anonymous Nicknames | Peers only see nicknames, not IPs               |
| 🚫 No Central Logging    | No data is stored remotely                      |
| 🔐 Host-only IP Exposure | Only host shares their IP/port to others       |

---

## 📚 What You'll Learn (and Show Off)

- 🧠 Python Networking (TCP sockets)
- 🧵 Multithreading for handling clients
- 🎨 Terminal UI with [`rich`](https://github.com/Textualize/rich)
- 🔐 AES-based encryption (`pycryptodome`)
- 🌐 P2P connection architecture
- 🔁 UPnP & NAT traversal basics
- 🧩 CLI argument parsing with `argparse`
- 📦 Packaging for `pip` with `setuptools`
- 🌍 Open-source development workflows

---

## 🚀 Usage & Installation

> Package it for quick installs and use via command-line:

### 📥 Install via pip (in future):
```bash
pip install p2pchat
````

### 🖥️ Host a Room

```bash
p2pchat --host 7788 --name Alice --password myroom
```

### 📡 Join a Room

```bash
p2pchat --join 1.2.3.4:7788 --name Bob --password myroom
```

---

## 🧪 Best Use Cases

* 👾 **Hackerspaces** & dev clubs
* 🎓 **College or LAN** group chat
* 🧑‍🤝‍🧑 **Friends-only chats** (fully local)
* 🕵️‍♂️ **Privacy-first communities**
* 🌍 **Chatting across NAT/firewalls** (with UPnP enabled)

---

## 💡 Future Ideas

* 📧 `.edu` email-based rooms
* 🔗 Invite codes with expiration
* 📈 WebSocket-based GUI frontends
* 📲 Mobile companion app (via QR invite)
* 🌐 Public Room Discovery (optional directory mode)

---

## 🧠 About This Project

This is a passion project meant to demonstrate:

* How terminal apps can still be powerful & elegant
* That encrypted, serverless chat is totally possible
* That Python is capable of networking, UI, and encryption together

---

> Want to contribute, fork, or star the project?
> Join us — this is open-source privacy, made simple.

---

