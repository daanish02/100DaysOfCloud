# Day 2 – Create an Azure Virtual Machine

## Problem Statement
The Nautilus DevOps team is planning to migrate a portion of their infrastructure to the Azure cloud incrementally. 
As part of this migration, you are tasked with creating an Azure Virtual Machine (VM).

The requirements are:

1. Use the existing resource group.
2. The VM name must be `devops-vm`, it should be in `West US` region.
3. Use the `Ubuntu 22.04 LTS` image for the VM.
4. The VM size must be `Standard_B1s`.
5. Attach a default Network Security Group (NSG) that allows inbound `SSH (port 22)`.
6. Attach a `30 GB` storage disk of type `Standard HDD`.
7. The rest of the configurations should remain as default.

After completing these steps, make sure you can SSH into the virtual machine.

## Objective
Create an Azure Virtual Machine and connect to it securely using SSH.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Virtual Machines** and open the service.
3. Click **Create** → **Azure virtual machine**.
4. Configure the **Basics** tab:
   - Select or create a **Resource Group**.
   - Enter a **Virtual Machine name**.
   - Choose the **Region**.
   - Select the **Image**.
   - Choose the **VM size**.
   - Configure **Inbound port rules** to allow SSH (Port 22).
5. Navigate to the **Disks** tab:
   - Select the **Disk type**.
   - Configure the required **Disk size**.
6. Skip the remaining optional configuration tabs.
7. Click **Review + Create**, then click **Create**.
8. Once deployment is complete, note the **Username** and **Public IP address** of the VM.
9. Connect to the VM using SSH:  
   ```bash
   ssh -i <ssh-key-path> <username>@<public_ip>
   ```

## Result
An Azure Virtual Machine is successfully created and accessed securely via SSH.
