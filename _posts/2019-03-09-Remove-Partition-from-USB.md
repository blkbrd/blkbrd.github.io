---
layout: post
title: "Remove Partition from USB"
date: 2019-03-09
---

Today I learned how to remove partition from a thumb drive (which I was way too excited about). 
open a command prompt, run <code>diskpart</code>, then <code>list disk</code>, select your USB thumbdrive with <code>select disk X</code> 
(where X cooresponds to your device. check out the size to verify you're picking the right one), 
look at existing partitions with <code>list partition</code>. From here you can either go through and delete what you want or use the check 
out existing partitions with <code>list partition</code>. From here you can either go through and delete what you want or use the 
<code>clean</code> if you dont want to select each partition. Once you're done with that, use <code>create partition primary</code> and youre
done! Exit with the <code>exit</code> command. 

I love sysadmin skills, lol!
