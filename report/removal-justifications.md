# Service and Package Removal Justifications

| Change | What did it expose? | What would break without it? | Status |
|---|---|---|---|
| CUPS | Print-service attack surface | Printing and print queues | Verify |
| Avahi | Multicast DNS and service discovery | LAN service discovery | Verify |
| Telnet server | Cleartext remote login | Legacy Telnet connections | Verify |
| FTP server | FTP file-transfer service | FTP workflows | Verify |
| Samba | SMB file-sharing service | SMB shares and integrations | Verify |

Update this table to reflect actual changes on the target VM.
