---
layout: post
title: "Python ctypes"
date: 2018-10-17
---

The ctypes module lets us load DLL files as libraries where we can ID load address and text segment!
<p>
<script>
  from ctypes import *
  import sys
  import string
  kernel32 = windll.kernel32
  windll.LoadLibrary(sys.argv[1])
  loadAddr = kernel32.GetModuleHandleA(sys.argv[1])
  print hex(loadAddr)
  print hex(loadAddr + 0x1000)
</script>

I learned about ctypes at SANS Exploit Writing class
