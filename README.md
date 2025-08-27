# PacketsDatabase.com Mirror

This repository provides a regularly updated mirror of IP addresses from [packetsdatabase.com](https://packetsdatabase.com/). The data is intended for security research, threat intelligence, and network monitoring.

## How It Works

This repository uses a GitHub Actions workflow to automatically fetch the complete dataset from the packetsdatabase.com API every **30 minutes**. The raw data is then processed into more accessible formats.

## Generated Files

The following files are generated and updated automatically:

### 1. Simple IP List

A plain text file containing one IP address per line. Useful for scripts and simple blocklists.

- **File**: [`ip_list.txt`](ip_list.txt)
- **Direct Link (Raw)**: `https://raw.githubusercontent.com/BlackSnowDot0/YOUR_REPO/main/ip_list.txt`

### 2. Zmap Blacklist Format

A configuration file formatted for use as a [Zmap](https://zmap.io/) blacklist. Each IP address is listed in CIDR notation (e.g., `192.168.1.1/32`).

- **File**: [`zmap_blacklist.conf`](zmap_blacklist.conf)
- **Direct Link (Raw)**: `https://raw.githubusercontent.com/BlackSnowDot0/YOUR_REPO/main/zmap_blacklist.conf`

---

*Disclaimer: This is an unofficial mirror. The data is provided "as is" and is sourced directly from the public API of packetsdatabase.com.*
