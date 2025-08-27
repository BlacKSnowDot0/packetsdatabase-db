# 📡 PacketsDatabase.com IP Mirror & Security Feeds

![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/BlacKSnowDot0/packetsdatabase-db/update_data.yml?branch=main&style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/BlacKSnowDot0/packetsdatabase-db?style=for-the-badge&color=brightgreen)
<!-- IP_COUNT_PLACEHOLDER -->

A continuously updated, automated mirror of malicious IP addresses sourced from [packetsdatabase.com](https://packetsdatabase.com/). This repository provides multiple ready-to-use blocklists and data feeds for security research, threat intelligence, and network defense.

---

## 📊 Live Statistics
*(Your charts will appear here if you are keeping that feature)*

| Top 10 ISPs                               | Protocol Distribution                             | TCP vs. UDP                                   |
| :---------------------------------------: | :-----------------------------------------------: | :-------------------------------------------: |
| ![Top 10 ISPs](isp_chart.png)             | ![Protocol Distribution](protocol_chart.png)      | ![TCP vs UDP](type_chart.png)                 |

---

## 📂 Available Feeds & Formats

All files are updated every 30 minutes. Use the "Raw Link" for automation.

### General Purpose Lists

| File                               | Description                                                               | Raw Link                                                                                     |
| :--------------------------------- | :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| `ip_list.txt`                      | A simple, newline-separated list of all unique IP addresses.              | `.../main/ip_list.txt`                      |
| `full_data.csv`                    | All records in CSV format for analysis in spreadsheets or databases.      | `.../main/full_data.csv`                    |
| `full_data.jsonl`                  | All records in JSON Lines format for easy programmatic parsing.           | `.../main/full_data.jsonl`                  |

### Firewall & Server Blocklists

| File                               | Description                                                               | Raw Link                                                                                     |
| :--------------------------------- | :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| `nginx_blocklist.conf`             | A drop-in blocklist for NGINX (`deny <ip>;`).                             | `.../main/nginx_blocklist.conf`             |
| `iptables_blocklist.sh`            | A shell script to add all IPs to an `iptables` DROP chain.                | `.../main/iptables_blocklist.sh`            |

### Targeted & Specialized Lists

| File                               | Description                                                               | Raw Link                                                                                     |
| :--------------------------------- | :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| `port_22_ssh.txt`                  | IPs observed attacking the SSH service (port 22).                         | `.../main/port_22_ssh.txt`                  |
| `port_3389_rdp.txt`                | IPs observed attacking the RDP service (port 3389).                       | `.../main/port_3389_rdp.txt`                  |
| `asn_summary.csv`                  | A summary of ASNs, ranked by the number of malicious IPs they host.       | `.../main/asn_summary.csv`                  |

*Replace `...` in the Raw Links with `https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO`*

---

## 💡 How To Use

```bash
# Example: Download the NGINX blocklist and include it in your configuration
wget -O /etc/nginx/blocklists/packetsdatabase.conf https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/nginx_blocklist.conf

# Then, in your nginx.conf http or server block:
# include /etc/nginx/blocklists/packetsdatabase.conf;
```

---

## ⚖️ Disclaimer

> This is an unofficial mirror. The data is sourced from the public API of [packetsdatabase.com](https://packetsdatabase.com/). Use this information responsibly.
