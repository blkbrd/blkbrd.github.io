---
layout: post
title: "Python ctypes"
date: 2018-10-17
---

The ctypes module lets us load DLL files as libraries where we can ID load address and text segment!
<p>
<code>
  from ctypes import *
</code>
<code>
  import sys
</code>
<code>
  import string
</code>
<code>  
  kernel32 = windll.kernel32
</code>
<code>
  windll.LoadLibrary(sys.argv[1])
</code>
<code>
  loadAddr = kernel32.GetModuleHandleA(sys.argv[1])
</code>
<code>
  print hex(loadAddr)
</code>
<code>
  print hex(loadAddr + 0x1000)
</code>
<p>
I learned about ctypes at SANS Exploit Writing class
