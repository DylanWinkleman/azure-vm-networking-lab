# Azure VM + Networking Lab 

## Overview
This project demonstrates how to deploy a Windows Virtual Machine in Microsoft Azure and securely configure networking access using a Virtual Network (VNet) and Network Security Group (NSG).

## Goals
- Deploy a Windows Server VM in Azure
- Understand the resources created with a VM (VNet, NIC, NSG, Public IP, Disk)
- Configure secure RDP access (port 3389) using NSG rules
- Practice proper cleanup to avoid unnecessary costs

## Azure Services Used
- Azure Virtual Machine (Windows Server)
- Virtual Network (VNet)
- Subnet
- Network Security Group (NSG)
- Public IP Address
- OS Disk

## Steps Completed
1. Created a Resource Group: `rg-az900-vm-lab`
2. Deployed a Windows Server VM: `vm-win-lab01`
3. Verified networking components were created (NIC, VNet, NSG, Public IP)
4. Connected to the VM using Remote Desktop (RDP)
5. Secured inbound access by restricting RDP (3389) to my IP address
6. Deleted the resource group to prevent ongoing charges

## Security Notes
- RDP access was restricted to my public IP only instead of allowing traffic from anywhere.
- This reduces exposure to unauthorized connection attempts from the internet.

## What I Learned
- A VM in Azure is made up of multiple resources working together (compute, storage, networking)
- NSG inbound rules act as the primary firewall for VM access
- Limiting access by IP is a basic best practice for security
- Resource Groups make it easy to delete everything when finished


- Resource Group overview
- VM overview
- NSG inbound rule showing RDP restricted to your IP


## Notes About Region / Image
I used the West Europe region and Windows Server 2025 Datacenter (Gen2) because my free Azure subscription did not allow deployment in my original region with older images.

## Screenshots

### Resource Group Created
github.com/DylanWinkleman/azure-vm-networking-lab/blob/main/screenshots/screenshots02-resource-group-created.png

### VM Overview
https://github.com/DylanWinkleman/azure-vm-networking-lab/blob/main/screenshots/screenshots01-vm-overview.png 

### NSG Rule (RDP restricted to my IP)
https://github.com/DylanWinkleman/azure-vm-networking-lab/blob/main/screenshots/screenshots03-nsg-inbound-rule.png



