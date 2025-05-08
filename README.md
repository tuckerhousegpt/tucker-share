
# tucker-share
basic file sharing site
=======
# Tucker Share

A secure, portable file hosting stack using:

- **Filebrowser** – Web-based file manager (via Docker)
- **Cloudflare Tunnel** – No-port-forward secure access
- **files.tucker.work** – Authenticated admin access (via Cloudflare Access)
- **share.tucker.work** – Public share link destination

---

## 🔧 Project Structure

tucker-share/
├── filebrowser/
│ └── docker-compose.yml
├── cloudflared/
│ └── config.yml
├── scripts/
│ └── start-share.sh
├── .gitignore
└── README.md


---

## 🚀 How to Start

From your terminal:

```bash
~/tucker-share/scripts/start-share.sh

This will:

    Start Filebrowser

    Run the Cloudflare tunnel
🔐 Cloudflare Setup

    files.tucker.work: Requires login via Cloudflare Access (@biztec.us)

    share.tucker.work: Open for public file access

To generate public links, log in via share. or manually swap domains in the link.
📦 To Do

    Auto-start tunnel on boot

    Multi-user support

    QR/link sharing tools

    Wirepod integration

>>>>>>> feb24b0 (Initial commit of file sharing stack)
