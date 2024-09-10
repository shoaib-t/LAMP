<h1>LAMP Stack Vulnerability Testing</h1>

<h2>Description</h2>
<p><b>This vulnerability assessment was a hands-on project involving Linux distributions. VirtualBox as the hypervisor of choice was utilized to run Ubuntu and Kali Linux. Settings were configured to assure no other devices on the network were impacted by this test.</b></p>

<p><b><i>Project Summary</i></b></p>

- Performed vulnerability assessment on a LAMP (Linux, Apache, MySQL, PHP) stack hosted web application within an Ubuntu virtual machine using Kali Tools for an in-depth analysis.
- Employed advanced tools, such as Nmap and Legion for comprehensive vulnerability scanning, and used Wireshark for network traffic analysis.
- Utilized Nikto for efficient detection of security threats, and proactively adhered to DISA-STIG recommendations for implementing security enhancements.

<hr/>

<h3>Languages Used</h3>

- <b>Python:</b> High Level Programming Language

<h3>Utilities Used</h3>

- <b>VirtualBox:</b> Hosted Hypervisor
- <b>Apache HTTP Server:</b> Web Server
- <b>MySQL:</b> Database Management System
- <b>Legion:</b> Network Penetration Testing Tool
- <b>Nikto:</b> Web Server Vulnerability Scanner
- <b>Nmap:</b> Network Scanner
- <b>Wireshark:</b> Packet Analyzer

<h3>Other Resources Used</h3>

- <b>CIS:</b> Ubuntu Linux 22.04 LTS Benchmark v1.0.0
- <b>OWASP:</b> Top Ten Proactive Controls 2018
- <b>STIG:</b> Canonical Ubuntu 20.04 LTS Security Technical Implementation Guide

<hr/>

<h2>Part 1: Ubuntu VM</h2>
	<h3>Simple Python Code & Apache Server</h3>
		<p align="center"><img src="https://github.com/user-attachments/assets/d38ca09c-f17d-430e-a4cb-9def57afdd71" height="85%" width="85%" alt="lamp-python"/></p>
		<p align="center"><img src="https://github.com/user-attachments/assets/f0a50cbd-2303-43be-bada-2778caac810c" height="85%" width="85%" alt="lamp-text-contents"/></p>
		<p align="center"><img src="https://github.com/user-attachments/assets/9f07b76d-a7dc-43f4-b424-baf1d5c91c5e" height="85%" width="85%" alt="lamp-apache"/></p>
	<h3>App Database Creation</h3>
		<p align="center"><img src="https://github.com/user-attachments/assets/fb0c92eb-2abf-441e-8030-81734dd48db6" height="85%" width="85%" alt="lamp-sql1"/></p>
		<p align="center"><img src="https://github.com/user-attachments/assets/03ae9cc9-8763-4803-867e-42bd52fddbf2" height="85%" width="85%" alt="lamp-sql2"/></p>

<hr/>

<h2>Part 2: Kali Linux VM</h2>
	<h3>Nmap Scan</h3>
		<p align="center"><img src="https://github.com/user-attachments/assets/28ab0408-027a-49a5-81e3-1ac08da37fa0" height="85%" width="85%" alt="lamp-nmap"/></p>
	<h3>Wireshark Scan</h3>
		<p align="center"><img src="https://github.com/user-attachments/assets/89c4907b-7072-40ad-87e0-d32f6400deef" height="85%" width="85%" alt="lamp-wireshark"/></p>
	<h3>Legion & Nikto Vulnerability Scan</h3>
		<p align="center"><img src="https://github.com/user-attachments/assets/15308bb5-441d-4897-b9f0-e907b15bad51" height="85%" width="85%" alt="lamp-legion"/></p>
		<p align="center"><img src="https://github.com/user-attachments/assets/3a537764-18c0-43a3-b794-0b03e3515ee2" height="85%" width="85%" alt="lamp-nikto"/></p>

<hr/>

<h2>Part 3: Following Security Control Recommendations</h2>
	<h3>CIS Ubuntu Linux 22.04<br/>LTS Benchmark v1.0.0 - 08-30-2022</h3>
		<b>1.3.1</b>
			<p align="center">Ensure AIDE is installed (Automated)</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/40565880-4764-4e4a-bc1a-8492ed304292" height="85%" width="85%" alt="cis1"/></p>
			<p align="center"><img src="https://github.com/user-attachments/assets/6daf35e4-d402-41e3-99e7-467d8fc07de2" height="85%" width="85%" alt="cis2"/></p>
	<h3>OWASP (Open Worldwide Application Security Project)<br/>Top Ten Proactive Controls 2018</h3>
		<b>C7</b>
			<p align="center">Enforce Access Controls</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/0311150d-4c07-4e80-a282-7fde9c93a97c" height="85%" width="85%" alt="owasp1"/></p>
	<h3>STIG: Canonical Ubuntu 20.04 LTS Security Technical Implementation Guide<br/>Version 1, Release 9</h3>
		<b>SV-238196r653763_rule</b>
			<p align="center">The Ubuntu operating system must provision temporary user accounts with an expiration time of 72 hours or less.</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/5ca1608d-48f5-4ee0-9bac-88a2165401fa" height="85%" width="85%" alt="stig1"/></p>
		<b>SV-238200r653775_rule</b>
			<p align="center">The Ubuntu operating system must allow users to directly initiate a session lock for all connection types.</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/18cdb1dd-26f4-4fc6-babf-8b4d2a65a957" height="85%" width="85%" alt="stig2"/></p>
		<b>SV-238204r832936_rule</b>
			<p align="center">Ubuntu operating systems when booted must require authentication upon booting into single-user and maintenance modes.</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/d47a5575-b753-47b6-a329-965833c9bde1" height="85%" width="85%" alt="stig3"/></p>
		<b>SV-238206r653793_rule</b>
			<p align="center">The Ubuntu operating system must ensure only users who need access to security functions are part of sudo group.</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/f5b08836-f2de-4e83-a401-a692d2876f43" height="85%" width="85%" alt="stig4"/></p>
		<b>SV-238208r853405_rule</b>
			<p align="center">The Ubuntu operating system must require users to reauthenticate for privilege escalation or when changing roles.</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/1a464ddc-cd0d-4ad9-be6a-a08fcff24fb3" height="85%" width="85%" alt="stig5"/></p>
		<b>SV-238238r853416_rule</b>
			<p align="center">The Ubuntu operating system must generate audit records for all account creations, modifications, disabling, and termination events that affect /etc/passwd.</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/8866dedb-a409-4d96-8295-d5d79991ec76" height="85%" width="85%" alt="stig6"/></p>
			<p align="center"><img src="https://github.com/user-attachments/assets/5fa95348-9b7f-4b7c-8beb-6c116dc8933e" height="85%" width="85%" alt="stig6.1"/></p>
			<p align="center"><img src="https://github.com/user-attachments/assets/505de99d-0890-4ed3-b783-3397fe424f49" height="85%" width="85%" alt="stig6.2"/></p>
		<b>SV-238245r653910_rule</b>
			<p align="center">The Ubuntu operating system must be configured so that audit log files are not read or write-accessible by unauthorized users.</p>
			<p align="center"><img src="https://github.com/user-attachments/assets/3e5dd160-600c-4979-a985-88da267e50cc" height="85%" width="85%" alt="stig7"/></p>
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
