# Lab 01 — Network Fundamentals & Basic Recon

## Objective
Build a strong foundation in networking by identifying host/network details and performing safe reconnaissance on a target domain/IP (legal/authorized targets only).

## What I Practiced
- IP addressing & subnet basics
- DNS basics (A/AAAA/CNAME/MX)
- Connectivity testing (ping, traceroute)
- Basic recon using safe commands/tools
- Documentation of findings and takeaways

## Tools Used
- Windows CMD / PowerShell (or Linux terminal)
- `ipconfig` / `ifconfig`
- `ping`
- `tracert` / `traceroute`
- `nslookup` / `dig`
- (Optional) `whois`, `nmap` (only on authorized targets)

## Steps & Evidence
### 1) Check local network configuration
- Command: `ipconfig /all` (Windows) or `ifconfig` (Linux)
- Evidence: Screenshot saved in `/Lab-01-Network-Fundamentals/screenshots/`

### 2) Test connectivity
- Command: `ping 8.8.8.8` and `ping google.com`
- Note: Difference between IP ping vs domain ping (DNS resolution)
- Evidence: Screenshot

### 3) Trace the route
- Command: `tracert google.com` (Windows) or `traceroute google.com` (Linux)
- Evidence: Screenshot

### 4) DNS lookup
- Command: `nslookup google.com`
- Evidence: Screenshot

## Key Takeaways
- DNS translates domain names into IP addresses.
- Traceroute helps visualize hops and latency across the path.
- Documenting outputs clearly is part of professional security work.

## Next Improvements
- Add a short subnetting practice section
- Run `whois` and document results (authorized targets)
- Add a small nmap scan example on a local lab VM
