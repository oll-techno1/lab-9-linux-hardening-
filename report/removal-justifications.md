# Service and Package Removal Justifications

| Change | What did it expose? | What would break? | Status |
|---|---|---|---|
| CUPS | Printing service attack surface | Printing and print queues | Verify |
| Avahi | Multicast DNS/service discovery | LAN discovery | Verify |
| Telnet server | Cleartext remote login | Legacy Telnet clients | Verify |
| vsftpd | FTP file-transfer service | FTP workflows | Verify |
| Samba | SMB file sharing | SMB shares and Windows integration | Verify |
| Other changes | Document actual exposure | Document actual impact | Verify |

Only list removals that were actually performed. Check dependencies
and operational requirements before removing any service.
