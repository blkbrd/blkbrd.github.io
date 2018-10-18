---
layout: post
title: "GDB Cheat Sheet"
date: 2018-10-18
---

GDB Cheat Sheet from [Rendition Infosec](https://www.renditioninfosec.com/ "Rendition Infosec")

Inspect the stack, displaying 20 double words at the ESP register

<code> x/20xw $esp </code>

Inspect the stack, displaying 32 bytes at the ESP register

<code> x/32b $esp </code>

Display a string at a given address

<code> x/s 0x41414141 </code>

Set a breakpoint at a givven address
<p><code> break *0x41414141 </code>

List breakpoints
<p><code> info break </code>

Delete a breakpoint
<code> del BREAKPOINT_NUMBER </code>

Disassemble a function
<code> disass FUNCTION </code>

Display register contents
<code> info reg </code>

Run with input from Python
<code> run > >(python -c 'print "A" * 16') </code>

Print a register
<code> print $esp </code>
