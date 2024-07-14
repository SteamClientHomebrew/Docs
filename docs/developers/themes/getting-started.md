---
sidebar_position: 2
---

# Getting Started

Here you'll learn a little bit about a template theme code base, and how to get ready to make a theme

### Creating a Template

Clone or download this [template repository](https://github.com/SteamClientHomebrew/Themes) and place it in your skins folder. 

### Getting Ready 

First things first. Boot up steam with parameters 
`-cef-enable-debugging -dev`. this enabled CEF Remote Debugging and Developer mode enabling to inspect element.

Navigate to http://localhost:8080/

- This allows you to see all inspect-able windows on the Steam Client. These names are useful when you need to select a certain window to insert CSS or JS into.

- It also allows you to skin the Overlay and SuperNav's and other windows you normally cant just inspect element on.


:::info

Note:
Some weird places to skin are the task-tray context menu, to skin that you need to right click the steam icon to open the context menu, then from there you need to right click empty space and click View Page Source this is really the only way you can see the HTML inside that window.

:::

Most other windows can be themed through CEF Remote Debugger, or by CTRL+SHIFT+I