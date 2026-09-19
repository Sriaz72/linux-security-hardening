# System Hardening Notes

## SSH

- Disabled direct root login over SSH.
- Disabled empty-password SSH authentication.
- Validated SSH configuration with `sshd -t`.
- Reloaded SSH after configuration changes.
- Verified SSH service status.

## Firewall

- Enabled UFW.
- Default incoming traffic policy: deny.
- Default outgoing traffic policy: allow.
- Allowed SSH.
- Allowed HTTP.
- Allowed HTTPS.

## Fail2Ban

- Installed Fail2Ban.
- Enabled the SSH jail.
- Configured authentication failure limits.
- Verified Fail2Ban service status.
- Verified SSH jail status.

## Auditing

Used Linux commands to inspect:

- Listening network ports
- Running services
- Firewall rules
- SSH configuration
- User accounts
- Sudo privileges
- Security-related logs

## Lessons Learned

Security hardening should be performed carefully and tested after every configuration change.

SSH configuration must be validated before reloading the service.

Firewall rules should be configured before enabling the firewall to prevent accidental loss of remote access.

Security controls should be verified using system commands rather than assuming that configuration changes worked.
