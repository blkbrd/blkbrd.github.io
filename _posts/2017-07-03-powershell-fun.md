---
layout: post
title: "Lillian Warner, powershell info 2"
date: 2017-07-03
---
<title>{{ page.title }}</title>
# Here are some fun powershell commands for when you can't touch a computer remotely

## Search Autostart
<blockquote><p> get-cimInstance win32_startupCommand | Select-Object name, command, location, user | format-list</p></blockquote>
## Logs
<blockquote><p> `$yesterday = (Get-Date) - (New-TimeSpan -Days 1)
Get-WinEvent -logname "Windows Powershell" | Where-Object {$_.TimeCreated -ge $yesterday}` </blockquote></p>
