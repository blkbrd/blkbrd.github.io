---
layout: post
title: "Lillian Warner, powershell info 2"
date: 2017-07-03
---
# Here are some fun powershell commands for gathering artifacts when you can't touch a computer remotely

## Search Autostart
<blockquote><p> <code>get-cimInstance win32_startupCommand | Select-Object name, command, location, user | format-list</code> </p>
</blockquote>

## Logs
<p>get log from the last day, i think</p>
<blockquote><p> <code>$yesterday = (Get-Date) - (New-TimeSpan -Days 1)
Get-WinEvent -logname "Windows Powershell" | Where-Object {$_.TimeCreated -ge $yesterday} </code></p>
</blockquote>

<p>count the number of events</p>
<blockquote><p><code>$events = get-winEvent -Logname "Windows Powershell"
$events.count</code> </p>
</blockquote>

<blockquote><p> <code>.....| Select-Object -First 100</code></p>
</blockquote>

## Drivers
<blockquote><p><code>Get-WindowsDriver -online -all
</code></p></blockquote>

## Directory Walk
<blockquote><p><code> Get-ChildItem -path <path> -recurse -force
</code></p><blockquote>

## Users
<blockquote><p><code>net user
</code></p><blockquote>

## Network
<blockquote><p><code>netstat.exe -ano
</code></p><blockquote>

## Process
<blockquote><p><code>Get-Process | Select-Object name, id, productversion, company
</code></p><blockquote>
