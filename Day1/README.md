# Day 1 Task - Nmap TCP SYN Scan & Wireshark Capture

This folder contains files related to Day 1 task of the Elevate LABS cybersecurity internship.

- Nmap scan results (`scan_results.txt`)
- Wireshark capture file (`scan_capture.pcapng`)
- Summary of the task and findings (this README)

###Day 1: Network Scan and Research on Open Ports

##Common Services Running on Open Ports (What I Found)
135/tcp (msrpc): This port is used by Microsoft RPC services on Windows. It is often targeted because it has some known vulnerabilities.

445/tcp (microsoft-ds): Used for SMB (file and printer sharing) on Windows. It is important but also often attacked by malware like WannaCry.

1042/tcp (afrog): An uncommon port that might be a custom service or misidentified. Needs further checking.

1043/tcp (boinc): BOINC is software for volunteer distributed computing (like SETI@home). This means some distributed computing might be running.

5357/tcp (wsdapi): Used by Windows to discover devices like printers on the network. It might expose some device info.

7778/tcp (interwise): Used by Interwise, a collaboration tool. Could be outdated or vulnerable depending on the version.

##Potential Security Risks Ports 135 and 445: High risk because attackers often exploit these ports to gain access or move inside networks.
Ports 1042 and 1043: Medium risk since these are less common and could be custom services with unknown vulnerabilities.

Port 5357: Medium risk as it might leak information about network devices.

Port 7778: Medium risk if the software is outdated and has known vulnerabilities.

##Additional Notes The host with IP 10.0.2.15 has all ports closed, which means it might be secured or not in use. Other hosts have the same open ports, probably because they are virtual machines cloned from the same image.

###Analyzing Network Traffic with Wireshark When I captured packets during the scan, I focused on TCP SYN packets because they are the first step in establishing connections. To do this in Wireshark, I used the filter:

tcp.flags.syn == 1 && tcp.flags.ack == 0

This filter shows only the initial SYN packets sent by Nmap during the TCP SYN scan, helping me clearly see the scanning traffic without other packet noise.
