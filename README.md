# 📡 PacketsDatabase.com IP Mirror

![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/BlacKSnowDot0/packetsdatabase-db/update_data.yml?branch=main&style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/BlacKSnowDot0/packetsdatabase-db?style=for-the-badge&color=brightgreen)
![IPs Tracked](https://img.shields.io/badge/IPs%20Tracked-313770-blue?style=for-the-badge)

A continuously updated, automated mirror of malicious IP addresses sourced from [packetsdatabase.com](https://packetsdatabase.com/). This repository provides ready-to-use blocklists for security research, threat intelligence, and network monitoring.

---

## ⚙️ How It Works

This repository is fully automated using a GitHub Actions workflow that runs every **30 minutes**. The process is simple:

1.  🤖 **Fetch**: The action calls the packetsdatabase.com API to get the latest complete dataset.
2.  📄 **Process**: It parses the massive JSON response to extract all unique IP addresses.
3.  📂 **Generate**: It creates multiple blocklist formats from the extracted data.
4.  🚀 **Commit**: The action pushes the updated files back to this repository, ensuring the data is always fresh.

---

## 📂 Available Files

The data is provided in the following formats for easy integration into your tools and scripts.

| File                                                | Description                                                          | Raw Link (for `curl`, `wget`, etc.)                                                                            |
| :-------------------------------------------------- | :------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------- |
| [`ip_list.txt`](ip_list.txt)                        | A plain text file with one IP per line. Ideal for simple scripts.    | `https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/ip_list.txt`                          |
---

## 💡 Usage Examples

You can easily use these files in your own projects. Here are a few examples:

### Download with `curl` or `wget`

```bash
# Download the simple IP list
curl -O https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/ip_list.txt

# Or using wget
wget https://raw.githubusercontent.com/BlacKSnowDot0/packetsdatabase-db/main/ip_list.txt
```

---

## ⚖️ Disclaimer

> This is an unofficial mirror. The data is provided "as is" and is sourced directly from the public API of [packetsdatabase.com](https://packetsdatabase.com/). Use this information responsibly.
