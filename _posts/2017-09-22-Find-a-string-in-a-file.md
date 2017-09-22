Recently, I needed to find a particular string within a bunch of csv files that were strewn across multiple folders. 
This command was my google'd solution, but I want to remember it: 

<code>
find . -iname '*.csv' -exec cat {} \; | grep THING-YOURE-LOOKING-FOR
</code>
