---
layout: post
title: "PowerShell Speach Synthesizer"
date: 2017-09-26
---

PowerShell has a speech synthesizer!
Here's a fun script to grab random phrases from a file and have your computer speak them!

<code>
Add-Type -AssemblyName System.speech
$speaker = New-Object System.Speech.Synthesis.SpeechSynthesizier
</code>

<code>
$Location = PATH
$Phrase = (Get-content $Location) | Get-Random
</code>

<code>
$speaker.rate = -2 #scale from -10 to 10
$speaker.Speak($Phrase)
</code>

<code>
#this also works:
#$speaker.Speak("hello, $env:USERNAME ")
</code>
