# 🐧 Linux Community Hackathon - Linux OpenHack’26 🚀

[![Linux](https://img.shields.io/badge/OS-Ubuntu%20Linux-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/)
[![Nginx](https://img.shields.io/badge/Web%20Server-Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)](https://nginx.org/)
[![Security](https://img.shields.io/badge/SSL%2FTLS-HTTPS%20Enabled-008080?style=for-the-badge&logo=letsencrypt&logoColor=white)](https://www.openssl.org/)
[![Status](https://img.shields.io/badge/Hackathon-Completed-brightgreen?style=for-the-badge)](https://github.com/kmsanthosh07/Linux_community_hackathon)

> **Official Documentation Repository** for **Linux OpenHack’26**, featuring comprehensive terminal workflows, network topology configurations, verified server logs, and complete screenshot proof for all 5 technical tasks.

---

## 📌 Candidate & Hackathon Metadata

| Parameter | Details |
| :--- | :--- |
| **Event Name** | Linux Community Hackathon - Linux OpenHack’26 |
| **Student Name** | **SANTHOSH KM** |
| **Roll Number** | **7376242AD293** |
| **Repository** | [`kmsanthosh07/Linux_community_hackathon`](https://github.com/kmsanthosh07/Linux_community_hackathon.git) |
| **Environment** | Ubuntu Linux (Oracle VirtualBox VM) / Nginx Web Server |

---

## 📊 Task Completion Matrix

| Task | Core Objective | Status | Documentation Link |
| :---: | :--- | :---: | :---: |
| **Task 1** | Set up Nginx server & host custom HTML template provided by organizers. | `✅ COMPLETED` | [Task 1 Documentation](./Task1/README.md) |
| **Task 2** | Access hosted web page from a remote client across LAN network. | `✅ COMPLETED` | [Task 2 Documentation](./Task2/README.md) |
| **Task 3** | Modify hosted HTML page remotely over SSH with student credentials. | `✅ COMPLETED` | [Task 3 Documentation](./Task3/README.md) |
| **Task 4** | Host a separate web application on port 8080 using Virtual Hosts. | `✅ COMPLETED` | [Task 4 Documentation](./Task4/README.md) |
| **Task 5** | Convert server to HTTPS (Port 443) using self-signed SSL certificate. | `✅ COMPLETED` | [Task 5 Documentation](./Task5/README.md) |

---

## 📂 Repository File Tree

```text
Linux_community_hackathon/
├── README.md                                  # Main Hackathon overview & portfolio documentation
├── Task1/
│   ├── README.md                              # Task 1 Nginx setup & terminal verification
│   ├── Screenshot 2026-10-07 230645.png       # Organizer HTML template preview
│   ├── Screenshot 2026-10-07 230651.png       # Nginx package installation log
│   ├── Screenshot 2026-10-07 230652.png       # Nginx service status & HTTP 200 header check
│   ├── Screenshot 2026-10-07 230678.png       # Web directory backup & chmod permission setup
│   ├── Screenshot 2026-10-07 230687.png       # Downloading index.html template via curl
│   └── Screenshot 2026-10-07 230699.png       # Final local HTTP verification
├── Task2/
│   ├── README.md                              # Task 2 LAN network connectivity details
│   ├── Screenshot 2026-10-07 230654.png       # Network ping reachability test from remote client
│   └── Screenshot 2026-10-07 230688.png       # Remote client curl header inspection
├── Task3/
│   ├── README.md                              # Task 3 Remote SSH modification details
│   ├── Screenshot 2026-10-07 230686.png       # Remote SSH connection & nano editing session
│   └── Screenshot 2026-10-07 230687.png       # Live webpage update verification in browser
├── Task4/
│   ├── README.md                              # Task 4 Nginx Virtual Host configuration (Port 8080)
│   ├── Screenshot 2026-10-07 230676.png       # Site configuration block & symlink setup
│   ├── Screenshot 2026-10-07 230685.png       # Active listening socket check via ss -lntp
│   ├── Screenshot 2026-10-07 230687.png       # Dual port browser side-by-side verification
│   └── Screenshot 2026-10-07 230690.png       # Remote client curl test on port 8080
└── Task5/
    ├── README.md                              # Task 5 SSL/TLS migration & HTTPS setup
    └── Screenshot 2026-10-07 230609.png       # HTTPS SSL certificate warning & curl -k verification
```

---

## ⚡ Task Implementation Summaries

### 🔹 Task 1: Nginx Web Server Setup & Custom HTML Hosting
- **Summary:** Installed Nginx web server, downloaded organizer custom HTML template to `/var/www/html/index.html`, set file permissions (`chmod 777`), validated configuration (`nginx -t`), reloaded Nginx daemon, and verified local HTTP HTTP/1.1 200 response.
- **Evidence:** 6 step-by-step terminal screenshots.

### 🔹 Task 2: Remote LAN Network Accessibility
- **Summary:** Configured server LAN IP (`10.10.144.102`), verified cross-machine reachability via `ping`, inspected HTTP response headers via `curl -I`, and confirmed browser access across local network.
- **Evidence:** 2 network verification screenshots.

### 🔹 Task 3: Remote HTML Modification via SSH
- **Summary:** Enabled OpenSSH server daemon (`sshd`), established secure remote SSH session, updated `/var/www/html/index.html` with Student Name (`SANTHOSH KM`) and Roll Number (`7376242AD293`), and verified live network updates.
- **Evidence:** 2 SSH editing & verification screenshots.

### 🔹 Task 4: Multi-Port Web Hosting (Port 8080)
- **Summary:** Provisioned separate document root `/var/www/task4/`, created custom virtual host configuration in `/etc/nginx/sites-available/task4`, bound port `8080`, verified active sockets (`ss -lntp`), and validated dual-port browser access.
- **Evidence:** 4 virtual host configuration screenshots.

### 🔹 Task 5: SSL/TLS Encryption & HTTPS Migration
- **Summary:** Generated 2048-bit RSA self-signed SSL certificate using `openssl`, updated Nginx site configuration for SSL listening on port `443`, reloaded Nginx, and verified secure access via `curl -k https://10.10.144.102`.
- **Evidence:** 1 SSL verification screenshot.

---

## 🛡️ Verification & Guidelines Compliance
All tasks were executed completely using Linux terminal commands adhering strictly to **Linux OpenHack’26** rules and standards.
