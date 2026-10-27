# Verification Summary

| Requirement | Evidence file | Expected result |
|---|---|---|
| Baseline snapshot | `normal-vm/before.txt` | Listening ports, running services, package count, SUID files |
| Final snapshot | `normal-vm/after.txt` | System state after hardening |
| Comparison | `normal-vm/diff.txt` | Differences between baseline and final state |
| Account audit | `normal-vm/account-audit.txt` | Account IDs, shells, password status, login history |
| SSH configuration | `normal-vm/sshd-effective.txt` | Effective SSH daemon settings |
| SSH validation | `normal-vm/ssh-validation.txt` | Configuration syntax check |
| ProxyJump | `client/config.example` | Router-based SSH access configuration |
| Update logs | `normal-vm/update-logs.txt` | Automatic update execution records |
| Port scan | `router/nmap-after.txt` | Services detected on the target |
| Authentication test | `client/password-auth-test.txt` | Password authentication rejected when disabled |

## Interpretation

A reduced listening-port list may indicate a smaller network attack surface.
Package counts and service lists provide additional context.

SSH syntax validation confirms that the configuration parses. A separate
connection test is required to verify authentication and ProxyJump.

Update logs should establish whether updates were installed or no eligible
updates were available.
