---
sidebar_position: 1
description: Quick guide to getting Millennium.
---

# Installing

## Windows

### Automatic
To install Millennium on windows, we use a PowerShell installer script. To run the script, open PowerShell, paste the following command, and press enter.

This installer is entirely open source and we encourage the community audit the [source code](https://steambrew.app/install.ps1). 

```powershell
iwr -useb "https://steambrew.app/install.ps1" | iex
```

<!-- #### Video Guide

<video width="100%" height="500" controls>
  <source src="https://cdn.discordapp.com/attachments/1242907596889919492/1263723521901723710/install.mp4?ex=669b45be&is=6699f43e&hm=e35582d01bcac0b0942038ba261c2e9739b70bcb45d2f39962ddee9aabe456f9&" type="video/mp4"/>
</video> -->

### Manual

Start by downloading all the files from [this repository](https://github.com/SteamClientHomebrew/Millennium/releases/latest). Simply put all files into your Steam directory, which you can find by running the PowerShell command below

```powershell
(Get-ItemProperty -Path "HKLM:\SOFTWARE\WOW6432Node\Valve\Steam" -Name "InstallPath").InstallPath
```
