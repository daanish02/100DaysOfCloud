# Day 22 – Configuring Instances with User Data in Azure

## Problem Statement
The Nautilus DevOps Team is working on setting up a new virtual machine (VM) to host a web server for a critical application. 
The team lead has requested you to create an Azure VM that will serve as a web server using Nginx. This VM will be part 
of the initial infrastructure setup for the Nautilus project. Ensuring that the server is correctly configured and accessible 
from the internet is crucial for the upcoming deployment phase.

As a member of the Nautilus DevOps Team, your task is to create a VM with the following specifications:
- Instance Name: The VM must be named `datacenter-vm`.
- Image: Use any available `Ubuntu image` to create this VM.
- Custom Script Extension/User Data: Configure the VM to run a custom script during its launch. This script should:
	- Install the `Nginx` package.
	- Start the Nginx service.
- Network Security Group (NSG): Ensure that the VM allows HTTP traffic on `port 80` from the internet.

## Objective
Configure an Azure Virtual Machine at launch using user data to automatically install and start Nginx.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open **Virtual Machines**.
3. Click **Create** and configure the VM:
   - Enter **Virtual Machine name**.
   - Select or create a **Resource Group**.
   - Choose the **Location**.
   - Select the **Image**.
   - Choose the **VM size**.
4. In **Inbound port rules**, allow **HTTP (Port 80)**.
5. Navigate to the **Advanced** tab.
6. Enable **User data**.
7. Paste the following bash script:
   ```bash
   #!/bin/bash
   apt update -y
   apt install -y nginx
   systemctl start nginx
   systemctl enable nginx
   ```
8. Click Review + Create, then click Create.
9. Once the VM is running, copy the Public IP address.
10. Paste the IP address into a web browser.

## Result
The Nginx default page is displayed in the browser, confirming successful VM configuration using user data.
