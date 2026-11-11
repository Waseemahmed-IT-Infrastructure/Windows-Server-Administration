
# Windows Server Administration

## Overview

This repository covers common Windows Server administration tasks, including server monitoring, Windows services, event logs, storage checks and basic troubleshooting.

## Administration Tools

- Server Manager
- Windows Services
- Event Viewer
- Task Manager
- Windows PowerShell
- Computer Management
- Windows Admin Center

## Server Health Monitoring

Common checks include:

- CPU and memory usage
- Available disk space
- Server uptime
- Network connectivity
- Windows service status
- System and application events
- Pending updates and restart requirements

## Windows Service Management

Windows services support operating system functions and enterprise applications.

Basic checks include:

1. Open Services.
2. Locate the required service.
3. Check its current status.
4. Review its startup type.
5. Check related dependencies.
6. Review event logs if the service fails.

Service restarts should follow approved operational procedures.

## Event Viewer

Event Viewer is useful for investigating server issues.

Important logs include:

- System
- Application
- Security
- Setup

When troubleshooting, review the event time, source, event ID and description.

## Disk and Storage Management

Common tasks include:

- Checking available disk capacity
- Reviewing disk volumes
- Monitoring storage warnings
- Investigating low disk space
- Checking disk health information

## Basic PowerShell Commands

### Check Computer Information

    Get-ComputerInfo

### Check Running Services

    Get-Service | Where-Object Status -eq 'Running'

### Check Disk Volumes

    Get-Volume

### Check Recent System Events

    Get-WinEvent -LogName System -MaxEvents 20

## Basic Troubleshooting

| Issue | What to Check |
|---|---|
| High CPU usage | Running processes and services |
| Low disk space | Volume usage and application logs |
| Service not starting | Dependencies and Event Viewer |
| Server unreachable | Network configuration and connectivity |
| Application error | Application logs and service status |
| Restart pending | Update status and maintenance schedule |

## Best Practices

- Monitor server health regularly.
- Follow approved change management procedures.
- Review logs before making changes.
- Confirm backups before major maintenance.
- Document troubleshooting results.
- Never publish real server names, IP addresses or credentials.

## Note

This repository contains general Windows Server administration documentation without company-specific infrastructure details.
