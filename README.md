<p align="center">
<img src="https://imgur.com/1aKhtZP.png"/>
</p>

<h1>NMAP Scanning In Kali Linux Lab </h1>
This tutorial gives a brief demonstration on how NMAP works. NMAP is a open-source command-prompt tool that can be used to identity the hosts, services, and version of OSs are running on a network as well as what ports they may have open. A few basic Nmap command will be executed within a Kali Linux ISO image in Vmware Player 17. We will be scanning the website scanme.nmap.org. This website allows users to scan the IP address associated with this website for educatinal purposes.
.<br />


<h2>Environments and Technologies Used</h2>

- Vmware Player 17
- Kali  Linux ISO Image
-Command Prompt

<h2>Operating Systems Used </h2>

- Kali Linux</b> 

<h2>Installation Steps</h2>

<p>Overview</p>

<p>
<img src = "https://imgur.com/tACTJXN.png" " height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
 <p>
1. First we will navigate to VMware Workstation 17 Player an open the Kali Linux ISO image VM.

</p>                                                                                                    
                                                                                                     
<p>
<img src= "https://imgur.com/vA0AE5t.png" " height="80%" width="80%" alt="Disk Sanitization Steps" />
</p>

<p>
                                                                                                 
                                                                                                 
2. Once navigated to the command prompt, type the command nmap scanme.nmap.org. Using this basic command, we were able to scan a single IP address on scanme.nmap.org to identify the specific port, port state, and service that this host is running.                                                                         
</p>
<br />




<p>
<img src="https://imgur.com/6KIeZt7.png" />
 />
"/>
</p>


<p>
<img src = "https://imgur.com/EPMw1dV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
3. The command "-sS" that is used for the scan scanme.nmap.org is TCP SYN scan or half-open/stealth scan. The commands by having NMAP first send out a TCP SYN packet to the targeted host. After the host responds with a SYN-ACK packet, NMAP then sends a RST packet to close the connection to the host rather than sending back a ACK packet. Here, we can see whether each port on the host is open or closed.
</p>
<br />



<p>
<img src = "https://imgur.com/Mhbqqqe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>



<p>
4. The command -sV that is used within nmap -sV scanme.nmap.org can be used to identify the versions of services that the host may be using. As we can see, the http protocol is using the verison of Apache htpd 2.4.7. This type of scan is helpful for identidying vulnerabilities when it comes to outdated services that  host may be running.

</p>
<br />


<p>
<img src="https://imgur.com/PROFgWc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


<p>
5. Next, let's try the command nmap -oN scanme.nmap.org. The "-oN" within this command will capture the results of the nmap scan and place the results within the file output.txt.

</p>
<br />


<p>
<img src="https://imgur.com/ioxBBDE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


6.  The last two commands we can try out are -sN and -sF. The command -sN apart of nmap -sN scanme.nmap.org sends TCP packets to ports without any flags set. The -sF commands sends TCP packets to the target host with the FIN set. For both types of scans used, we can see that nmap wausn't able to determine the state of the ports that were scanned. These scans are typically used when you want to be more stealthy with your scans, so firewall associated with the hpst may have blocked these types of scans.
