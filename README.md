# SSH Remote Server Setup

**Project Page:** https://roadmap.sh/projects/ssh-remote-server-setup

## Overview
Configured a secure remote access environment using OpenSSH on an Ubuntu Linux server. Generated Ed25519 cryptographic keys to establish secure, passwordless authentication and locked down the SSH daemon configuration to reject standard password-based logins, hardening the server against brute-force attacks.

## Features
* OpenSSH server deployment
* Ed25519 cryptographic key generation and authorization
* Hardened `sshd_config` security parameters
* Local secure connection testing
## Proof of Execution
Successfully authenticated into the locked-down server using the Ed25519 cryptographic key, bypassing password prompts entirely:

```bash
gold@gold:/mnt/c/Users/lucko/OneDrive/Desktop/Nginx-Project$ ssh gold@localhost
Welcome to Ubuntu 26.04 LTS (GNU/Linux 6.18.33.2-microsoft-standard-WSL2 x86_64)

System load:  0.05               Processes:             54
Usage of /:   0.2% of 1006.85GB  Users logged in:       0
Memory usage: 10%                IPv4 address for eth0: 172.30.55.151

gold@gold:~$
