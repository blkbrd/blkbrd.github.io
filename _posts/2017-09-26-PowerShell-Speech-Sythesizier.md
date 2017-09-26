PowerShell has a speech synthesizier!
Here's a fun script to grab random phrases from a file and have your computer speak them!

<code>
Add-Type -Assemblyman System.speech
$speaker = New-Object System.Speech.Synthesis.SpeechSynthesizier

$Location = PATH
$Phrase = (Get-content $Location) | Get-Random

$speaker.rate = -2 #scale from -10 to 10
$speaker.Speak($Phrase)

#this also works:
#$speaker.Speak("hello, $env:USERNAME ")
</code>
