# Linux Security Hardening Lab

## Overview

This project demonstrates practical Linux security hardening and system administration using Debian GNU/Linux 13 in a VMware virtualized environment.

The lab focuses on securing a Linux server through SSH configuration, firewall administration, Fail2Ban, system auditing, security logging, and troubleshooting.

## Environment

- Debian GNU/Linux 13
- VMware
- Bash
- OpenSSH
- UFW
- Fail2Ban
- systemd
- Git/GitHub

## Objectives

- Harden SSH access
- Configure a host-based firewall
- Protect SSH against repeated authentication failures
- Review running services and listening ports
- Audit users and administrative privileges
- Review security-related system logs
- Document security configurations and troubleshooting procedures

## Security Hardening

### SSH Hardening

The SSH service was hardened by:

- Disabling direct root login over SSH
- Disabling empty-password authentication
- Validating the SSH configuration before applying changes
- Verifying the SSH service after configuration changes

Commands used:

```bash
sudo sshd -t
sudo sshd -T
sudo systemctl status ssh

