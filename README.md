# My Self-Hosted Home Lab

A resilient, private, and secure on-premises infrastructure designed to eliminate dependence on third-party cloud providers, maximize data privacy, and upgrade my enterprise IT skills.

---

## Project Philosophy & Goals

* **Complete Independence:** No Google Cloud, no Netflix, no YouTube Ads.
* **Privacy & Transparency:** Regaining absolute control over network telemetry and data protocols.
* **Cost Efficiency:** Offsetting long-term subscription fees through self-hosted alternatives.
* **Skill Leveling:** Continuous hands-on training in security architectures, networking, and virtualization.

---

## Core Services & Components

### Networking & Security
* **Firewall (pfSense/OPNsense):** Custom policy enforcement to gain deep visibility into inbound and outbound WAN traffic.
* **VPN (WireGuard/Tailscale):** Secure, encrypted remote access to home dashboards and internal resources from anywhere.
* **AdBlocker (Pi-hole / AdGuard Home):** Network-wide DNS sinkholing to block intrusive trackers and ads.

### Data & Infrastructure
* **NAS (Network Attached Storage):** Centralized file sharing for household users and trusted friends.
* **Password Manager (Vaultwarden):** Self-hosted Bitwarden backend to secure credentials without cloud exposure.
* **Uninterruptible Power Supply (UPS):** Automated, graceful shutdown sequences during critical power events.

### Media, Web, & Entertainment
* **Streaming Platform (Plex/Jellyfin):** On-demand media server to replace commercial streaming providers.
* **Web Hosting:** A small sandbox web server hosted locally for testing and fun.

### Compute, Virtualization, & AI
* **Virtual Machines & Containers:** High-availability virtualization layer (e.g., Proxmox/ESXi) running Linux/Windows nodes and Docker.
* **Local AI (Ollama):** Private LLM processing to automate, categorize, and parse emails or calendars locally.
* **BTC Miner Dashboard:** A dedicated telemetry dashboard tracking a small Bitcoin mining operation.

### Sustainability
* **PV Modules (Solar):** Integrated solar power telemetry to maintain a green energy profile for the lab.

---

## Key Infrastructure Requirements

To keep the system robust and reliable, the architecture adheres to these core pillars:

* **High Availability:** Implementing **VRRP** (Virtual Router Redundancy Protocol) for router/gateway resilience.
* **Physical On-Premises Security:** Utilizing physical locks and strict local password management.
* **Edge Security:** Hardened firewall rules with **zero open ports** directly exposed to the public internet (relying on VPN/reverse proxies).
* **Network Segmentation:** Strict VLAN isolation separating **Trusted Devices**, **Guest Networks**, and untrusted **IoT Components** (cameras, smart appliances).
* **Data Protection:** Automated scheduled backups and system snapshot retention policies.

---