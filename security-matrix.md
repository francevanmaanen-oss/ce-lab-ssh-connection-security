# Security Configuration Matrix
 
## Instance Details
- Instance ID: i-xxxxxxxxxxxxx
- Instance Type: t3.micro
- Public IP: -------
- Private IP: -----
 
## Security Group: week2-web-server-sg
 
### Inbound Rules
| Protocol | Port | Source | Purpose | Risk Level |
|----------|------|--------|---------|------------|
| TCP | 22 | 0.0.0.0/0 | SSH access | Medium |
| TCP | 80 | 0.0.0.0/0 | Web traffic | Low |
 
### Outbound Rules
| Protocol | Port | Destination | Purpose |
|----------|------|-------------|---------|
| All | All | 0.0.0.0/0 | Unrestricted egress |
 
## Security Assessment
- HTTP accessible (200 OK)
- SSH working with key authentication
- ICMP blocked (ping test failed as expected)
- Port 3306 closed
- No unnecessary ports open
 
## Recommendations
1. Restrict SSH access to specific IP
2. Enable monitoring (CloudWatch)
3. Consider AWS Session Manager
