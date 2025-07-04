VPN Security Objective The goal of this task was to understand how VPNs (Virtual Private Networks) function to protect user privacy and encrypt internet traffic. This hands-on exercise involved setting up a VPN, verifying IP masking, testing encryption, and summarizing key insights.

🔧 Steps Performed Selected and Installed a Free VPN: I chose a reputable free VPN provider, created an account, and installed the VPN client on my machine.

Connected to a VPN Server: After installation, I connected to a nearby server location to ensure low latency and better performance.

Verified IP Address Change: I visited whatismyipaddress.com to check that my real IP address was successfully masked by the VPN server.

Confirmed Encrypted Traffic:

Browsed HTTPS websites to check that data was encrypted.

Used dnsleaktest.com to confirm there were no DNS leaks and all traffic was routed through the VPN.

Optional test with Wireshark showed traffic was scrambled (encrypted), meaning it couldn’t be easily interpreted by third parties.

Disconnected VPN and Compared Performance: I disconnected the VPN and noted changes in IP address and browsing speed. As expected, the VPN connection was slightly slower due to encryption and rerouting overhead.

Researched Encryption and Privacy Features: I learned that VPNs use protocols like OpenVPN, WireGuard, and encryption like AES-256 to ensure data is unreadable during transit. I also explored privacy features like:

Kill switches

No-log policies

DNS and IP leak protection

Summarized Benefits and Limitations:

Benefits:

Protects personal data on public Wi-Fi.

Hides your real IP address from websites and ISPs.

Access to geo-blocked or restricted content.

Helps maintain anonymity for sensitive activities.

Limitations:

Slight decrease in browsing speed.

Doesn’t protect against malware, phishing, or browser fingerprinting.

Free VPNs may log data or display ads.

Some websites block known VPN IP ranges.

📘 Conclusion This task helped me practically understand how VPNs contribute to network security and privacy. I learned how to use IP testing, DNS leak tools, and encryption principles to verify protection. The experience highlighted the importance of encryption in today’s digital world, especially when using untrusted networks.
