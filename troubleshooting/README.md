# Security Hardening Troubleshooting

## Overview

This document records troubleshooting procedures used during the Linux security hardening project.

The goal was to identify configuration problems, verify security services, and confirm that changes were applied successfully without disrupting server access.

## 1. SSH Configuration Problems

### Check SSH Configuration

Before reloading SSH after making configuration changes:

```bash
sudo sshd -t
