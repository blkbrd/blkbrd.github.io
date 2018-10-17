---
layout: post
title: "PortProxy"
date: 2017-06-23
---
<p>
PortProxy can be used as a native way to do tunnelling on Windows. How neat is that? <a href="https://youtu.be/Hm3JodBR-vs?t=21s">That's pretty neat!</a>
</p>
<p><code> netsh interface portproxy show all </code>
</p>
<p><code> netsh interface portproxy set v4tov4 &lt;listenport&gt; &lt;connectaddress&gt; &lt;connectport&gt; &lt;listenaddress&gt; &lt;protocol&gt;
<p>
<meta name="description" content="using command line to tunnel in Windows">
