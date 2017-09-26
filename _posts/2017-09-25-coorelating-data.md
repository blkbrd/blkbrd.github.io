Today I was faced with correlating data from one file (IDs) with columns in another file (columns of IDs and hostnames).
I know how I would do it in Excel, but I wanted to script it so I could repeat it quickly and often. 
I figured I was going to have to loop through the data, but I knew there MUST be a better, faster way.
Grep to the rescue! I was able to use <code> grep -F -f FILE DEST </code> to grep the fixed strings from a file. I sorted the file first.
It resulted in a fast match of the hostnames that matched the IDs located in the first file.  

I will post the full script in the next day or so
