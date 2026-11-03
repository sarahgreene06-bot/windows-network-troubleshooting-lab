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
- DNS servers resolve domain names 



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
Command:
`nslookup google.com`
## DNS and Connectivity Testing
### Observed Results

**Command:** `nslookup google.com`

- Domain: google.com
- IPv4: 142.250.65.78
- IPv6: 2607:f8b0:4006:804::200e
- Result: Successful DNS resolution

**Command:** `ping google.com`
- Result: Received ICMP replies

**Command:** `ping 8.8.8.8`
- Result: Received ICMP replies

### Troubleshooting Conclusion

I verified that DNS returned IPv4 and IPv6
addresses for google.com.

Both ping tests received ICMP replies,
demonstrating connectivity to the tested
destinations.

These tests do not confirm whether HTTP
or HTTPS services are functioning.
### Objective
Understand the difference between DNS resolution
and network connectivity.

### Commands Used
- `nslookup google.com` — Queries DNS.
- `ping google.com` — Resolves a name and
  tests for ICMP replies.
- `ping 8.8.8.8` — Tests ICMP responses
  directly by IP address.

### Observed Results
- nslookup: Output still needs verification.
- ping google.com: Received replies.
- ping 8.8.8.8: Received replies.

### What I Learned
DNS resolves domain names into IP addresses.
Ping checks whether a destination responds
to ICMP requests. Pinging an IP directly
does not require DNS.

### Conclusion
Both ping tests received replies.
This does not guarantee that websites
are accessible through HTTP or HTTPS.
Results:


## Lessons Learned
[Explain what you learned about DNS, DHCP,
IP addressing, and network troubleshooting.]

## Screenshots
[Add sanitized screenshots after completing the lab.]

## Project Status
In Progress
