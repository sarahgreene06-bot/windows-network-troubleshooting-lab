Windows Network Configuration and Troubleshooting Lab

Project Overview

In this project, I used Windows Command Prompt to examine my computer’s network settings, test connectivity, and understand how DNS works.

My goal was to practice basic networking commands used by IT Help Desk technicians when diagnosing connectivity problems.

Tools Used

* Windows Command Prompt
* ipconfig
* ping
* nslookup
* tracert

1. Inspect IP Configuration

Command: ipconfig /all

Purpose: Identify my computer’s network configuration.

My Findings:

* IPv4 Address: 192.168.12.238
* Subnet Mask: 255.255.255.0
* Default Gateway: 192.168.12.1
* DHCP Enabled: Yes
* DNS Server: 192.168.12.1

What I Learned:

I learned how to identify my computer’s IP address, subnet mask, default gateway, and DNS settings. DHCP was enabled, meaning my computer was configured to obtain network settings automatically.

2. Test Network Connectivity

Purpose: Determine whether my computer could communicate with devices on my local network and external networks.

Test A: Default Gateway

Command: ping 192.168.12.1

Results:

* Packets sent: 4
* Packets received: 4
* Packet loss: 0%
* Average response time: 1 ms

Conclusion: My computer successfully communicated with the default gateway.

Test B: External IP Address

Command: ping 1.1.1.1

Results:

* Packets sent: 4
* Packets received: 4
* Packet loss: 0%
* Average response time: 32 ms

Conclusion: My computer successfully received responses from an external IP address without needing DNS resolution.

Test C: Google Domain

Command: ping google.com

Results:

* Packets received: 4
* Successful ICMP replies

Conclusion: My computer successfully resolved the hostname and received responses from the destination.

Additional Connectivity Test

Command: ping 8.8.8.8

Result: Received ICMP replies.

Conclusion: The external IP address responded to my connectivity test.

3. Test DNS Resolution

Command: nslookup google.com

Purpose: Check whether DNS could translate a domain name into IP addresses.

Observed Results:

* Domain: google.com
* IPv4: 142.250.65.78
* IPv6: 2607:f8b0:4006:804::200e
* Result: Successful DNS resolution

Conclusion:

DNS successfully returned IPv4 and IPv6 addresses for google.com.

I learned that DNS converts domain names into IP addresses so computers can locate network destinations.

4. Trace Network Route

Command: tracert google.com

Purpose: Identify the network hops used to reach the destination.

Results:

* Traceroute completed
* Used IPv6
* Reached the destination in 11 hops

Conclusion:

I learned that tracert helps identify the path network traffic takes toward a destination. It can help technicians investigate where communication delays or failures may occur.

5. Troubleshooting Analysis

The tests showed that:

* My computer had a private IPv4 address and DHCP was enabled.
* My default gateway responded successfully.
* External IP addresses responded to ICMP requests.
* DNS successfully resolved google.com.
* Traceroute completed and showed the network path.

These results showed that the tested network functions were working at the time of testing.

However, successful ping tests do not guarantee that websites or other services are functioning correctly.

6. Lessons Learned

This project helped me understand the difference between IP configuration, network connectivity, and DNS resolution.

I learned that an IT technician should troubleshoot in steps instead of assuming what is wrong.

For example, if a computer can ping an external IP address but cannot resolve a website’s domain name, DNS may be the problem.

I also learned how to use Command Prompt results to document and explain my findings.

7. Screenshots

Add screenshots of the completed Command Prompt tests after hiding identifying or sensitive information.

8. Project Status

Core network configuration, connectivity, DNS, and traceroute testing completed.

README documentation and screenshots being finalized.