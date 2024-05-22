---
sidebar_position: 3
description: When things don't go as expected.
---

# Troubleshooting

- #### Error getting webSocketDebuggerUrl: 
  Another program is using Port 8080, run this command in CMD to find out what it is and terminate it
 
  `for /f "tokens=5" %a in ('netstat -aon ^| findstr 8080') do wmic process where processId=%a get ExecutablePath`

- #### Failed to install Millennium 
  Install the Millennium Binaries manually you can get them [here](https://github.com/ShadowMonster99/millennium-steam-binaries/releases) Download both 
  files and copy them to this directory/folder 

  `C:\Program Files (x86)\Steam`

- #### Installed, but not showing in Settings: 
  Please make sure you are not on any Beta branches of steam; this includes the Steam Beta Update & 
  Steam Families Beta. you can find out more [here](https://github.com/SteamClientHomebrew/Millennium#you-must-use-steam-stable-until-further-notice) 
  
  (**this notice will be removed after Millenniums next update**)

- #### Entry Point Not Found Error. 
  Windows 7 & 8.1 are no longer supported please update to windows 10 or 11

- #### Java Script Error
  Install the Millennium Binaries manually you can get them [here](https://github.com/ShadowMonster99/millennium-steam-binaries/releases) download both files and copy them to this directory/folder

  `C:\Program Files (x86)\Steam`