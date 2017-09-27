---
layout: post
title: "Coorelating Data with grep -F"
date: 2017-09-25
---

Today I was faced with correlating data from one file (IDs) with columns in another file (columns of IDs and hostnames).
<p>
I know how I would do it in Excel, but I wanted to script it so I could repeat it quickly and often. 
I figured I was going to have to loop through the data, but I knew there MUST be a better, faster way.
<p>
Grep to the rescue! I was able to use <code> grep -F -f FILE DEST </code> to grep the fixed strings from a file. I sorted the files first.
<p>
It resulted in a fast match of all the hostnames that matched the IDs located in the first file.  
