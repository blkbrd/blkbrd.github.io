---
layout: post
title: "Bypassing PowerShell Execution Policy"
date: 2017-09-22
---

So it turns out when Powershell tells you that you can't execute scripts, you may be able to just tell it to 'go away'
In a PowerShell prompt, type
<code>
cmd /c powershell /executionpolicy bypass "path-of-script-you-want-to-execute"
</code>
There are other fun switches you can uses like '-nop' for 'no profile', '/WindowStyle hidden' and you may use 'unrestricted' instead of 'bypass' as execution policy. 
