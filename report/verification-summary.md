# Verification Summary

| Requirement | Evidence | Status |
|---|---|---|
| Baseline snapshot | normal-vm/before.txt | Captured if file exists |
| Post-hardening snapshot | normal-vm/after.txt | Pending |
| Diff | normal-vm/diff.txt | Pending |
| Account audit | normal-vm/account-audit.txt | Collected |
| Package changes | normal-vm/removed-packages.txt | Collected if available |
| SSH settings | normal-vm/sshd-effective.txt | Collected |
| SSH validation | normal-vm/ssh-validation.txt | Collected |
| ProxyJump | client/config.example | Configuration template |
| Update logs | normal-vm/update-logs.txt | Collected if available |
| Nmap | router/nmap-after.txt | Pending target identification |
| Password authentication test | client/password-auth-test.txt | Pending |

Mark a test successful only after its output confirms success.
