---
layout: post
title: "rdesktop file transfer"
date: 2017-07-03
---
<p> While connecting, use this syntax to share a folder (or entire directory) on your local machine to a remote computer </p>
<blockquote><code>rdesktop -r disk:&lt;new sharename&gt;=/&lt;local path to share&gt; &lt;ip&gt;</code></blockquote>
<p> when logged into the remote machine, open a file explorer and navigate to the share via the given &lt;new sharename&gt;. I didnt check to see what additional artifacts are left from this session compared to a regualr rdesktop connection

