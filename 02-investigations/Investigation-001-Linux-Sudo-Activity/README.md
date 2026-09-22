# Investigation 001 — Linux Sudo Activity

## Overview

This investigation analyzes privileged command activity recorded in the Ubuntu authentication logs.

The objective was to identify who executed privileged commands, what commands were executed, and whether the activity was consistent with authorized administrative behavior.

## Environment

- OS: Ubuntu 26.04.1 LTS
- Environment: WSL 2
- Log source: `/var/log/auth.log`
- Account investigated: `cyberbountie.`

## Evidence Collected

The account identity was verified using:

```bash
id
sudo grep -a "sudo:" /var/log/auth.log | tail -15

/usr/bin/whoami
/usr/bin/tail -20 /var/log/auth.log
/usr/bin/tail -10 /var/log/auth.log
