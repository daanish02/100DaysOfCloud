# Day 10 – Attach Public IP to Azure Virtual Machine

## Problem Statement
The Nautilus DevOps team has already set up a virtual machine and allocated 
a public IP address. The final task is to attach this public IP 
to the VM's network interface card (NIC).

An existing VM named `devops-vm-pip` and a public IP address 
named `devops-pip` already exist.

- Attach the public IP `devops-pip` to the network interface 
of the VM `devops-vm-pip`.
- Make sure the VM is properly assigned the public IP.

## Objective
Associate an existing public IP address with an Azure Virtual Machine.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open the target **Virtual Machine**.
3. Stop the virtual machine.
4. Search for and open the **Public IP address** resource.
5. Click **Associate**.
6. Select **Resource type** and change it as required.
7. Select the appropriate **Resource name** (network interface).
8. Apply the association.
9. Navigate to the associated virtual machine overview.
10. Start the virtual machine.

## Result
The public IP address is successfully associated with the Azure Virtual Machine and active after restart.
