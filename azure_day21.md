# Day 21 – Assigning Public IP to Azure Virtual Machines

## Problem Statement
The Nautilus DevOps Team has received a new request from the Development Team to set up a new Azure Virtual Machine (VM). This VM will be 
used to host a new application that requires a stable public IP address. To ensure that the VM has a consistent public IP, 
a Static Public IP address needs to be associated with it. The VM will be named datacenter-vm, and the Static Public IP will be named 
datacenter-pip. This setup will help the Development Team to have a reliable and consistent access point for their application.

- Create an `Azure VM` named `datacenter-vm` using any available `Ubuntu image`, with the VM size `Standard_B1s`.
- Generate an `SSH public key` on the azure-client host and associate it with the VM for SSH access.
- Associate a `Static Public IP` address named `datacenter-pip` with this VM.
- Ensure the VM is accessible via SSH using the generated public key.

## Objective
Create an Azure Virtual Machine, manage public IP resources, and verify SSH connectivity using a reassigned public IP.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open **Virtual Machines**.
3. Click **Create** and configure the VM:
   - Enter **Virtual Machine name**.
   - Select or create a **Resource Group**.
   - Choose the **Image**.
   - Select the **VM size**.
4. On the local host machine, generate an SSH key pair.
5. Paste the SSH public key in the VM authentication settings.
6. Click **Review + Create**, then click **Create**.
7. Search for and open **Public IP addresses**.
8. Select the default public IP associated with the VM and **Disassociate** it.
9. Create a new **Public IP address** by providing a name and required settings.
10. Associate the new public IP with the **Network Interface (NIC)** of the VM.
11. From the local host machine, verify SSH access using the new public IP address.

## Result
The Azure Virtual Machine is successfully associated with a new public IP address, and SSH connectivity is verified.
