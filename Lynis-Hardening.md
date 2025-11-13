 Lab 01 – System Hardening Audit with Lynis

**Tool:** Lynis  
**Platform:** Kali Linux  
**Command Run:** `sudo lynis audit system`

---

## Summary of Findings

- SSH root login is enabled — recommended to disable.
- No active firewall detected — suggest configuring `ufw` or `iptables`.
- File permissions on `/etc/passwd` could be hardened.
- Suggest disabling unused services like `rsh`, `rexec`, and `talk`.
- Missing password complexity requirements.
- No integrity check tool (like AIDE) found installed.

---

## Next Steps (Recommendations)

- Edit `/etc/ssh/sshd_config` to set `PermitRootLogin no`.
- Enable `ufw`: `sudo ufw enable`, and add rules.
- Harden file permissions for critical system files.
- Install AIDE for file integrity monitoring.
- Review and disable unnecessary services.
