+++
description = "Splashtop is a remote monitoring and management (RMM) tool. More information will be added as it becomes available."
title = "Splashtop"
weight = 10
displayTitle = "Splashtop"
+++


{{< block "grid-1" >}}
{{< column "mt-2 pt-1">}}

# Splashtop


### Description

Splashtop is a remote monitoring and management (RMM) tool. More information will be added as it becomes available.

**Author**: Nasreddine Bencherchali



### Details


#### PE Metadata


- **Free**: No

- **Verification**: No




#### Installation Paths
- `C:\Program Files (x86)\Splashtop\*`
- `*\Splashtop\Splashtop Remote\Client for RMM\*`
- `strwinclt.exe`

### Forensic Artifacts

#### Disk Artifacts
- **File**: `C:\windows\System32\winevt\Logs\Splashtop-Splashtop Streamer-Status%4Operational.evtx`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\windows\System32\winevt\Logs\Splashtop-Splashtop Streamer-Remote Session%4Operational.evtx`
  **Description**: N/A
  **OS**: Windows
- **File**: `%PROGRAMDATA%\Splashtop\Temp\log\FTCLog.txt`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\log\agent_log.txt`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\log\SPLog.txt`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\log\svcinfo.txt`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\log\sysinfo.txt`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\SRService.exe`
  **Description**: Splashtop Remote Service
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\SRAgent.exe`
  **Description**: SplashTop Remote Agent
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Software Updater\SSUAgent.exe`
  **Description**: Splashtop Updater
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\SRUtility.exe`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\SRFeature.exe`
  **Description**: N/A
  **OS**: Windows
- **File**: `C:\Program Files (x86)\Splashtop\Splashtop Remote\Server\db\SRAgent.sqlite3`
  **Description**: N/A
  **OS**: Windows

#### Event Log Artifacts
- Event Details:
  - **Event ID**: 7045
  - **Provider Name**: Service Control Manager
  - **Log File**: System.evtx
  - **Service Name**: Splashtop Software Updater Service
  - **Image Path**: "C:\\Program Files (x86)\\Splashtop\\Splashtop Software Updater\\SSUService.exe"
  - **Description**: Service installation event as result of Splashtop Software Updater Service installation.
- Event Details:
  - **Event ID**: 7045
  - **Provider Name**: Service Control Manager
  - **Log File**: System.evtx
  - **Service Name**: Splashtop® Remote Service
  - **Image Path**: "C:\\Program Files (x86)\\Splashtop\\Splashtop Remote\\Server\\SRService.exe"
  - **Description**: Service installation event as result of Splashtop Remote Service installation.
- Event Details:
  - **Event ID**: 7045
  - **Provider Name**: Service Control Manager
  - **Log File**: System.evtx
  - **Service Name**: SplashtopRemoteService
  - **Image Path**: "C:\\Program Files (x86)\\Splashtop\\Splashtop Remote\\Server\\SRService.exe"
  - **Description**: Service installation event as result of Splashtop Remote Service installation.

#### Registry Artifacts
- **Path**: `KLM\SOFTWARE\WOW6432Node\Splashtop Inc.\*`
  **Description**: Splashtop Inc. registry key
- **Path**: `HKLM\SOFTWARE\WOW6432Node\Microsoft\Windows\CurrentVersion\Uninstall\Splashtop Software Updater`
  **Description**: Splashtop Software Updater uninstall key
- **Path**: `HKLM\SYSTEM\CurrentControlSet\Services\SplashtopRemoteService`
  **Description**: Splashtop Remote Service registry key
- **Path**: `HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\WINEVT\Channels\Splashtop-Splashtop Streamer-Remote Session/Operational`
  **Description**: Splashtop Streamer Remote Session event log channel
- **Path**: `HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\WINEVT\Channels\Splashtop-Splashtop Streamer-Status/Operational`
  **Description**: Splashtop Streamer Status event log channel
- **Path**: `HKLM\SOFTWARE\WOW6432Node\Microsoft\Windows\CurrentVersion\Uninstall\Splashtop Software Updater\InstallRefCount`
  **Description**: Splashtop Software Updater install reference count
- **Path**: `HKLM\SYSTEM\CurrentControlSet\Control\SafeBoot\Network\SplashtopRemoteService`
  **Description**: Splashtop Remote Service safe boot configuration
- **Path**: `HKU\.DEFAULT\Software\Splashtop Inc.\*`
  **Description**: Default user Splashtop Inc. registry key
- **Path**: `HKU\SID\Software\Splashtop Inc.\*`
  **Description**: User-specific Splashtop Inc. registry key
- **Path**: `HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Print\Printers\Splashtop PDF Remote Printer`
  **Description**: Splashtop PDF Remote Printer configuration
- **Path**: `HKLM\SOFTWARE\WOW6432Node\Splashtop Inc.\Splashtop Remote Server\ClientInfo\*`
  **Description**: Splashtop Remote Server client information

#### Network Artifacts

- **Description**: N/A
  **Domain**:
    `*.splashtop.com`

  **Port**: `N/A`




### References
- [https://www.synacktiv.com/publications/legitimate-rats-a-comprehensive-forensic-analysis-of-the-usual-suspects.html](https://www.synacktiv.com/publications/legitimate-rats-a-comprehensive-forensic-analysis-of-the-usual-suspects.html)

### Acknowledgements
- Théo Letailleur (in/theosyn)

{{< /column >}}
{{< /block >}}