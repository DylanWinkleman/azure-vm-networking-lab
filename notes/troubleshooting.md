# Troubleshooting Notes 

## Problem: Can't connect using RDP
### Checks
1. Confirm VM state is Running
2. Confirm VM has a Public IP
3. Check NSG inbound rule allows TCP 3389
4. Restrict NSG Source to "My IP"
5. Confirm correct username/password

## Problem: VM deployed but slow
- Check VM size (B-series is cheaper but slower)
- Check CPU usage
