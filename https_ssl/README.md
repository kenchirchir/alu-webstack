# HTTPS SSL Project

## Overview
This project focuses on securing website traffic by implementing HTTPS with SSL termination and enforcing HTTPS redirection. Key components include configuring subdomains, setting up HAProxy for SSL termination, and writing Bash scripts to audit DNS records.

## Learning Objectives
- Understand the two main roles of HTTPS SSL
- Recognize the importance of encrypting traffic
- Define SSL termination and how it works with HAProxy

## Requirements
- **System:** Ubuntu 16.04 LTS
- **Scripts:** Must pass Shellcheck (version 0.3.7) without errors
- **HAProxy:** Version 1.5 or higher for SSL termination

## Tasks

### 0. World Wide Web
Configure DNS subdomains for `www`, `lb-01`, `web-01`, and `web-02`:
- Add subdomains to point to their respective IPs.
- Write a Bash script to retrieve information on subdomains, using `dig` and `awk`.

#### Usage
```bash
./0-world_wide_web <domain> [subdomain]

