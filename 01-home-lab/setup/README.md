# Lab Setup

## Ubuntu Linux Endpoint

Ubuntu was deployed using Windows Subsystem for Linux 2 (WSL 2).

### Environment

| Component | Configuration |
|---|---|
| Operating System | Ubuntu 26.04.1 LTS |
| Virtualization | WSL 2 |
| Kernel | 6.18.33.2-microsoft-standard-WSL2 |
| Linux User | cyberbountie |
| Host | Windows 11 |

### Verification

WSL status was verified from PowerShell:

```text
NAME      STATE     VERSION
Ubuntu    Running   2

Linux environment was verified using:
uname -a
cat /etc/os-release
### Purpose

This Ubuntu endpoint will serve as a controlled Linux system for practicing:

- Linux security log analysis
- Authentication and SSH investigation
- Process and file investigation
- Threat hunting
- Detection testing
- SOC investigation workflows
