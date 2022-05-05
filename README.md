## Proof-of-Concept Exploit
### Description
The Pritunl VPN Client service is vulnerable to an arbitrary file write as SYSTEM on Windows. This is due to insecure directory permissions on the Pritunl ProgramData folder. The arbitrary file write is then able to be leveraged for full privilege escalation due to the privileged Pritunl VPN service executing commands as SYSTEM without specifying the full path of the executable.  
