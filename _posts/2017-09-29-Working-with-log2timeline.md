
I was dealing with some big .csv log2timeline output files recently.
Even with post-processing, the files were overflowing Excel.
I split the file on a Linux box ( <code> split -l LINES FILE </code> ).
Later I found some hex in an event log. Used <code> echo HEX | xxx -r -p </code> to convert back.
Nothing groundbreaking, but I thought I would write it down so I would remember it!
