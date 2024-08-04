---
sidebar_position: 1
description: Quick guide to getting Millennium.
---

# Installing

## Windows

### Automatic
To install Millennium on windows, we use a PowerShell installer script. To run the script, open PowerShell, paste the following command, and press enter.

This installer is entirely open source and we encourage the community audit the [source code](https://github.com/SteamClientHomebrew/Millennium/blob/main/scripts/install.ps1). 

```powershell
iwr -useb "https://raw.githubusercontent.com/SteamClientHomebrew/Millennium/main/scripts/install.ps1" | iex
```

### Manual

Start by downloading the Millennium's Windows assets from [this repository](https://github.com/SteamClientHomebrew/Millennium/releases/latest) under the name ` millennium-v0.0.0-windows-x86_64.zip `. Simply put all files into your Steam directory, which you can find by running the PowerShell command below

```powershell
(Get-ItemProperty -Path "HKLM:\SOFTWARE\WOW6432Node\Valve\Steam" -Name "InstallPath").InstallPath
```

## Linux

### Automatic
**Shell (pre-built binary)**

This installer is entirely open source and we encourage the community audit the [source code](https://github.com/SteamClientHomebrew/Millennium/blob/main/scripts/install.sh). 

```bash
curl -fsSL "https://raw.githubusercontent.com/SteamClientHomebrew/Millennium/main/scripts/install.sh" | sh
```

### Manual

Start by downloading the Millennium's Linux assets from [this repository](https://github.com/SteamClientHomebrew/Millennium/releases/latest) under the name ` millennium-v0.0.0-linux-x86_64.tar.gz `. Simply put all files into your Steam directory, which should be `~/.local/share/Steam/`