---
layout: post
title: "Powershell Keylogger"
date: 2017-09-12
---

[Aaron](http://aaronmreyes.com/ "Aaron's Webpage"), made a cool PowerShell-based keylogger 
(well, it *was* python until i bribed him to re-write it for me...) 

It is located on [ his GitHub page](https://github.com/a-rey/bitflip/tree/master/keylogger "Aaron's Keylogger")

It great because it handles the keylogging and the exfiltration of data!

In order to use it you: 
1. Create a fake Google Account (or use a throw-away)
2. Create a Spreadsheet in that account's Google Drive
3. Make the Sheet public
..1. <code> File > Share... > Give it a random name > Get sharable link </code>
4. Visit [Google Scripts](https://www.google.com/script/start/) and paste in the code from [server.gs](https://raw.githubusercontent.com/a-rey/bitflip/master/keylogger/server.gs)
5. Add the Sheet's URL from step 3.1 to the <code> SPREADSHEET_URL </code> variable in <code>server.gs </code>
..1. remove the <code> ?usp=sharing </code> at the end. URL should end in <code> /edit <code> 
6. Publish the server: 
..1. Save and name the project
..2. <code> Publish > Deploy as web app </code>
..* Make sure <code> Anyone, even anonymous </code> can access the app
..3. <code> Review permissions > </code> (your fake accout here) <code> > Advanced > Go to Untitled Project (unsafe) > </code> enter 'Continue' <code> > allow </code>
..4. Copy the URL and paste it in the <code> SERVER_URL </code> of the logger you are using
7. Copy the [powershell code](https://raw.githubusercontent.com/a-rey/bitflip/master/keylogger/windows/logger.ps1) to your victim
8. Run the powerShell script! 
..* The script runs for 1 to 3 minutes before publishing the keystrokes to the Google Sheet
9. Lastly, I went into the Google Sheet and published it to the web for easier viewing

Sometimes if I typed too fast, it doesnt record all of the typed keys, and it doesnt record backspaces or punctuation. 

Also, it only runs once and if you want it to continuously run, it needs some edits or perhaps a scheduled task to get it going again

Neat little tool! Thanks Aaron!
