# 📡 PacketsDatabase.com IP Mirror & Security Feeds

![GitHub Workflow Status](htthttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main//img.shieldshttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/githttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/actihttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/workfhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/stahttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/BlacKSnowDhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/packetsdatabasehttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/update_data.yml?branch=main&style=for-the-badge)
![GitHub last commit](htthttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main//img.shieldshttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/githttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/last-comhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/BlacKSnowDhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/packetsdatabase-db?style=for-the-badge&color=brightgreen)
<!--START_IP_COUNT_BADGE-->
![IPs Tracked](htthttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main//img.shieldshttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/bahttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/IPs%20Tracked-313791-blue?style=for-the-badge)
<!--END_IP_COUNT_BADGE-->

A continuously updated, automated mirror of malicious IP addresses sourced from [packetsdatabase.com](htthttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main//packetsdatabase.https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/). This repository provides multiple ready-to-use blocklists and data feeds for security research, threat intelligence, and network defense.

---

## 📂 Available Feeds & Formats

All files are updated every 30 minutes. Use the "Raw Link" for automation.

### General Purpose Lists

| File                               | Description                                                               | Raw Link                                                                                     |
| :--------------------------------- | :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| `ip_list.txt`                      | A simple, newline-separated list of all unique IP addresses.              | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/ip_list.txt`                      |
| `full_data.csv`                    | All records in CSV format for analysis in spreadsheets or databases.      | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/full_data.csv`                    |
| `full_data.jsonl`                  | All records in JSON Lines format for easy programmatic parsing.           | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/full_data.jsonl`                  |

### Firewall & Server Blocklists

| File                               | Description                                                               | Raw Link                                                                                     |
| :--------------------------------- | :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| `nginx_blocklist.conf`             | A drop-in blocklist for NGINX (`deny <ip>;`).                             | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/nginx_blocklist.conf`             |
| `iptables_blocklist.sh`            | A shell script to add all IPs to an `iptables` DROP chain.                | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/iptables_blocklist.sh`            |

### Targeted & Specialized Lists

| File                               | Description                                                               | Raw Link                                                                                     |
| :--------------------------------- | :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| `port_22_ssh.txt`                  | IPs observed attacking the SSH service (port 22).                         | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/port_22_ssh.txt`                  |
| `port_3389_rdp.txt`                | IPs observed attacking the RDP service (port 3389).                       | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/port_3389_rdp.txt`                  |
| `asn_summary.csv`                  | A summary of ASNs, ranked by the number of malicious IPs they host.       | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/asn_summary.csv`                  |

*Replace `...` in the Raw Links with `htthttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main//raw.githubusercontent.https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/YOUR_USERNhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/YOUR_REPO`*

---

## 💡 How To Use

```bash
# Example: Download the NGINX blocklist and include it in your configuration
wget https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/nghttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/blocklihttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/packetsdatabase.conf htthttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main//raw.githubusercontent.https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/BlacKSnowDhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/packetsdatabasehttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/mhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/nginx_blocklist.conf

# Then, in your nginx.conf http or server block:
# incluhttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/nghttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/blocklihttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/packetsdatabase.conf;
```

---

## ⚖️ Disclaimer

> This is an unofficial mirror. The data is sourced from the public API of [packetsdatabase.com](htthttps://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main//packetsdatabase.https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/). Use this information responsibly.
