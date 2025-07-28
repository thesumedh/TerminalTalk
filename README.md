You’re building a peer-to-peer, encrypted chat app that works directly in the terminal, without any central server — just invite code, IP+port, and raw sockets.

🔧 Key Features You Defined:
One host creates a room and shares IP:PORT#password (invite code)

Others join by entering the invite code

No servers or cloud services involved

Optional manual IP & port entry

Special support for .edu email access (future idea)

Host is the relay (acts like a lightweight server)

Nickname-only identity (no IP leaks for peers)

AES-encrypted messaging with room password

Local message logs (.txt)

Host can kick users

Terminal UI via rich library

No dependency on Ngrok or paid tools

UPnP (optional) for port auto-forwarding

📦 Architecture
P2P hybrid model:

Host acts as relay/server for the room

Others connect directly to host’s IP:port

No central service or API

Encryption handled via shared password and AES-256

Logs and configs saved locally only

🔐 Security Model:
End-to-end encryption using pycryptodome

Messages only visible to participants in the room

Nicknames shown instead of IPs

IP only required for the host

No data stored or sent to external servers

📚 Learning Outcomes
By building this project, you’ll learn:

Python sockets (TCP)

Multithreading

Terminal UI with rich

Encryption with AES

P2P architecture

NAT traversal concepts

Basic port forwarding / UPnP

CLI argument parsing (argparse)

Packaging with pip / setuptools

Open-source structure (GitHub organization, docs)

🔧 Deployment + Use Case
Can be packaged as a CLI tool:

css
Copy
Edit
pip install p2pchat
p2pchat --host 7788 --name Alice --password myroom
p2pchat --join 1.2.3.4:7788 --name Bob --password myroom
Each instance runs in the terminal, lightweight and fast

Suited for:

Hackerspaces

Local/college networks

Friends chatting securely

Anyone avoiding centralized chat platforms
