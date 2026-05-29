# 💥 ScottsTechX Hydra

<p align="center">
  <img src="https://img.shields.io/badge/Hydra-Login-Cracker-00ff88?style=for-the-badge&logo=linux&logoColor=black" alt="Hydra"/>
  <img src="https://img.shields.io/badge/Open-Source-00ff88?style=for-the-badge&logo=github&logoColor=black" alt="Open Source"/>
</p>

> **Network login brute-forcer — crack SSH, FTP, HTTP, SMB, and 50+ protocols.**

---

## ⚡ What It Does

Hydra performs rapid parallel brute-force attacks against login services — test password strength, audit authentication systems, recover forgotten passwords.

**For authorized testing only.**

## 🚀 Quick Usage

```bash
# SSH brute force
hydra -l admin -P passwords.txt ssh://target.com

# FTP login
hydra -l ftp -P wordlist.txt ftp://target.com

# HTTP Form POST
hydra -l admin -P passwords.txt target.com http-post-form "/login:user=^USER^&pass=^PASS^:F=Invalid"

# Parallel attack (32 tasks)
hydra -l admin -P passwords.txt -t 32 ssh://target.com

# Username list + password list
hydra -L users.txt -P passwords.txt smb://target.com
```

## 🎯 Common Targets

| Service | Command |
|---------|---------|
| SSH | `hydra -l user -P pass.txt ssh://target` |
| FTP | `hydra -l user -P pass.txt ftp://target` |
| HTTP | `hydra -l user -P pass.txt http-get://target` |
| SMB | `hydra -l user -P pass.txt smb://target` |

---

MIT © 2026
