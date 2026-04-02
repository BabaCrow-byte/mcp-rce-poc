# MCP RCE Proof of Concept - CVE-2026-23744

## Description
This script is a proof-of-concept for testing potential remote command execution (RCE) in an MCP `/api/mcp/connect` endpoint.

It sends a crafted JSON payload that may trigger command execution via server-side handling of shell commands.

⚠️ This tool is intended for **educational and authorized security testing only**.

---

## Features
- Checks target reachability
- Sends crafted MCP connect payload
- Executes user-provided command (if vulnerable)
- Displays response output

---

## Requirements
- Python 3.7+
- requests

Install dependencies:

```bash
pip install -r requirements.txt
```
##Usage

```bash
python3 exploit.py <target_ip> "command"
```
##Example

```bash
python3 exploit.py 10.10.10.5 "id"
```
