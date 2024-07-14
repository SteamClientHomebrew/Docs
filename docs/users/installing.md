---
sidebar_position: 1
description: Quick guide to getting Millennium.
---

# Installing

## Windows

### Automatic
To install Millennium on windows, we use a PowerShell installer script. To run the script, open PowerShell, paste the following command, and press enter.

This installer is entirely open source and we encourage the community audit the [source code](https://steambrew.app/install.ps1). 

```ps1
iwr -useb https://steambrew.app/install.ps1 | iex
```

### Manual

Start by downloading all the files from [this repository](https://github.com/SteamClientHomebrew/Millennium/releases/latest). Simply put all files into your Steam directory, which you can find by running the PowerShell command below

```ps1
(Get-ItemProperty -Path "HKLM:\SOFTWARE\WOW6432Node\Valve\Steam" -Name "InstallPath").InstallPath
```
