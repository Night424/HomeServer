# Home Server Project

This repository documents my personal **self-hosted home server** built on an old laptop and managed with **Docker + Portainer**.

The goal of this project is to learn Linux, Docker, self-hosting, and server management while running useful real-world services like media streaming, file storage, monitoring, and game servers.

This repo contains **configuration files, stack definitions, and documentation** — not personal data or media.

---

## Hardware

- Laptop server
- CPU: Intel i5-1035G1
- RAM: 8 GB DDR4
- Storage: 256 GB SSD
- OS: Ubuntu Server
- Network: Wi-Fi


## Core

All services are run using **Docker**, managed via **Portainer**.

## Currently running services:

| Service | Purpose | Port |
|------|--------|------|
| Jellyfin | Media server (movies, shows, music) | 8096 |
| File Browser | Web file manager | 8080 |
| Uptime Kuma | Service uptime monitoring | 3001 |
| Portainer | Docker container management | 9443 |
| System Monitoring | Host-level monitoring (non-container) | 9090 |

---

## Jellyfin Media Structure
Movies
movies/
- Movie Name (Year)/
   - Movie Name (Year).mp4
TV Shows
shows/
- Show Name/
   - Season 01/
      - Show Name S01E01.mp4
Music
music/
- Artist/
   - Album/
      - 01 Track Name.mp3

---

## Monitoring
Uptime Kuma
Monitors service availability (HTTP, TCP, Ping)
- Alerts when services go down
- Lightweight and easy to manage

### System Monitoring
Host-level monitoring for CPU, RAM, disk, and network

Used to keep an eye on laptop health (temps, load, storage)

---

## Security (In Progress)
-SSH hardening
-Firewall rules (UFW)
-Fail2Ban
-Docker volume isolation
-No services exposed publicly yet
-Remote access planned (Tailscale)

---

## What Is NOT In This Repo
this repository does not include:
- Media files
- Databases
- Passwords or secrets
- SSH keys
- Personal user data

All sensitive values are replaced with placeholders.

## Future Plans
Nextcloud (storage)

Game server hosting

Remote access

HTTPS

Automated backups

More monitoring & alerting

Documentation improvements

Improved hardware