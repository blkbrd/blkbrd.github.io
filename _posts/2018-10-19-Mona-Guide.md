
Guide to using Mona with Immunity Debugger

* ALT-L : open log window 
* !mona : type in text box and hit enter to get options and commands
* !mona help COMMAND : mor einfo about a particular command
* !mona update 
* !mona modules : display modules
* !mona config -set workingfolder C:\LOCATION : set location for output
* !mona jmp -r esp -m MODULE_NAME : search for trampolines and other code reuse blocks
* !mona seh -m MODULE_NAME : search SEH overwrite code sequences
* !mona pattern_create SIZE : create string to determine buffer size
* !mona pattern_offset PATTERN || !mona po PATTERN : locate location in pattern/string
* !mona rop : find ROP gadgets
