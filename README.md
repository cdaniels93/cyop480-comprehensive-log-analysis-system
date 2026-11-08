# Comprehensive Automated Log Analysis System

## Project overview

I built a lab system that collected logs from Linux, Windows, and a web server, converted them into a common format, searched for suspicious patterns, and sent results to Splunk and a local email alert.

---

## 1. Windows scheduled log export

Created a Windows Scheduled Task to run `export_events.ps1` every five minutes. The task appears as Ready, showing that it was registered and available to run.

![PowerShell showing the Windows scheduled log-export task](01-windows-scheduled-export-task.png)

---

## 2. Automated log collection

Ran `log_collect.py` on Ubuntu and verified that the Kali authentication log, Windows security events, and web access log were present.

![Ubuntu terminal showing log collection and the retrieved log files](02-log-collection.png)
