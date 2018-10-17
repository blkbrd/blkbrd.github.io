---
layout: post
title: "Working with log2timeline csv"
date: 2017-09-29
---

I was dealing with some big .csv log2timeline output files recently.
Even with post-processing, the files were overflowing Excel.
I split the file on a Linux box ( <code> split -l LINES FILE </code> ).
<p>
Later, I found some hex in an event log. I used <code> echo HEX | xxx -r -p </code> to convert back.
<p>
Nothing groundbreaking, but I thought I would write it down so I would remember it!
