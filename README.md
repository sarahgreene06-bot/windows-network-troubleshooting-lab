
### 1. Inspect IP Configuration

**Command used:**
`ipconfig /all`

**Purpose:**
To examine the network settings assigned to
my Windows computer and identify whether
DHCP is enabled.

**My findings:**
- IPv4 Address: 192.168.12.238
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.12.x
- DHCP Enabled: Yes
- DNS Servers: 192.168.12.x

**Troubleshooting analysis:**
- My computer's IPv4 address is used to
  communicate on the local network.
- The subnet mask helps identify which
  addresses are on the local network.
- The default gateway routes traffic to
  other networks.
- DHCP automatically assigns network
  configuration when enabled and available.
- DNS servers resolve domain names to
  IP addresses.




### My Conclusion

I used ipconfig /all to check my computer's
network settings.

My network settings appear normal so far.
Next, I will test connectivity and DNS.

### 2. Test Connectivity

**Purpose:**
To test whether my computer can communicate
with itself, an external IP, and a website.

**Commands:**
- `ping 127.0.0.1`
- `ping 1.1.1.1`
- `ping google.com`

**Results:**
[To be completed]

### 3. Test DNS
### 3. Test DNS
Command:
`nslookup google.com`

Results:
[To be completed]

## Troubleshooting Analysis
[Explain what each result tells you.]

## Lessons Learned
[Explain what you learned about DNS, DHCP,
IP addressing, and network troubleshooting.]

## Screenshots
[Add sanitized screenshots after completing the lab.]

## Project Status
In Progress
