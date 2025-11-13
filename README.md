#  Defensive Portfolio - Lab 01: Lynis Hardening with Dradis Report

##  Overview
This lab demonstrates a basic **Linux system hardening assessment** using [`Lynis`](https://cisofy.com/lynis/) — a popular open-source security auditing tool — followed by documentation and reporting using the **Dradis Community Edition**.

The goal of this lab is to:
- Perform a baseline scan of a Linux host using Lynis.
- Capture and interpret key hardening suggestions.
- Upload and document the scan inside Dradis.
- Generate and export a professional report.
- Upload the full lab to GitHub for public portfolio presentation.
-
--- ##  Tools Used
| Tool | Purpose | |--------------|---------------------------------------------|
| **Lynis** | System auditing and hardening recommendations |
| **Dradis CE**| Collaborative reporting and documentation |
| **Kali Linux** | OS environment used for scanning and documentation |
| **GitHub** | Version control and portfolio hosting |
--- ## Scan Summary 
### Key Findings - SSH configuration not hardened (missing Banner, Protocol version, root login enforcement). - Permissions on `/etc/passwd` and `/etc/shadow` not optimal. - Kernel hardening modules not fully enabled.
### Recommendations - Configure SSH with stronger security parameters. - Enforce restrictive file permissions on critical system files. - Enable kernel modules such as AppArmor or SELinux. - Disable unused services and unnecessary users. - Regularly audit the system using Lynis or equivalent tools.
