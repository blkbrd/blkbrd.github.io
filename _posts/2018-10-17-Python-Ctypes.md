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
  <p>
<code>
  import sys
</code>
    <p>
<code>
  import string
</code>
      <p><p>
<code>  
  kernel32 = windll.kernel32
</code>
        <p>
<code>
  windll.LoadLibrary(sys.argv[1])
</code>
          <p>
<code>
  loadAddr = kernel32.GetModuleHandleA(sys.argv[1])
</code>
            <p>
<code>
  print hex(loadAddr)
</code>
              <p>
<code>
  print hex(loadAddr + 0x1000)
</code>
<p>
I learned about ctypes at SANS Exploit Writing class
