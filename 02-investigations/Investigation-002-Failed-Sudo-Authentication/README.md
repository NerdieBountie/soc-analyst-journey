# Investigation 002 — Failed Sudo Authentication

## Overview

This investigation examines a failed local sudo authentication event recorded on an Ubuntu endpoint.

The objective was to determine the affected account, authentication source, frequency of failures, and whether the event indicated suspicious activity.

## Environment

- OS: Ubuntu 26.04.1 LTS
- Environment: WSL 2
- Log source: `/var/log/auth.log`
- Account: `cyberbountie`

## Detection

The event was identified by searching the authentication log for failed authentication events:

```bash
sudo grep -a "authentication failure" /var/log/auth.log


