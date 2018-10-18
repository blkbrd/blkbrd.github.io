

GDB Cheat Sheet from Rendition infosec 

Inspect the stack, displaying 20 double words at the ESP register
x/20xw $esp

Inspect the stack, displaying 32 bytes at the ESP register
x/32b $esp

Display a string at a given address
x/s <addr>

Set a breakpoint at a givven address
break *0x<rest of the address>

List breakpoints
info break

Delete a breakpoint
del <breakpoint number>

Disassemble a function
disass <func>
