---
layout: post
title: "GDB Cheat Sheet"
date: 2018-10-18
---

GDB Cheat Sheet from Rendition infosec 

Inspect the stack, displaying 20 double words at the ESP register
<code> x/20xw $esp </code>

Inspect the stack, displaying 32 bytes at the ESP register
<code> x/32b $esp </code>

Display a string at a given address
<code> x/s <addr> </code>

Set a breakpoint at a givven address
<code> break *0x<rest of the address> </code>

List breakpoints
<code> info break </code>

Delete a breakpoint
<code> del <breakpoint number> </code>

Disassemble a function
<code> disass <func> </code>

