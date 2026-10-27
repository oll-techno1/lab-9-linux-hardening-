Linux Hardening — Removal Justifications
========================================

| Change | Exposure reduced | Potential impact |
|---|---|---|
| CUPS | Printing service exposure | Printing unavailable |
| Avahi | Multicast DNS discovery | Local discovery may fail |
| Telnet server | Cleartext remote login | Telnet clients cannot connect |
| vsftpd | FTP service exposure | FTP transfers unavailable |
| Samba | SMB file sharing | SMB shares unavailable |

Remove only services that are unnecessary for the system's role.
