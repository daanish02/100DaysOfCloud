# Day 9 – Attach Network Interface Card (NIC) to Azure Virtual Machine

## Problem Statement
The Nautilus DevOps team is migrating services to Azure. 
They are breaking down tasks to ensure better control and 
optimization. You are tasked with attaching an existing 
network interface (NIC) to a virtual machine (VM).

An existing VM named `datacenter-vm` and a network interface 
named `datacenter-nic` already exist in the `West US` region.

- Attach the network interface `datacenter-nic` to the VM 
`datacenter-vm`.
- Ensure the NIC's status is `attached` before submitting the task.
- Make sure that the virtual machine initialization has 
been completed before submitting this task.

## Objective
Attach an existing Network Interface Card (NIC) to an Azure Virtual Machine.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open the target **Virtual Machine**.
3. Stop the virtual machine  
   > A VM must be stopped before attaching a network interface.
4. In the VM menu, navigate to **Networking** → **Network settings**.
5. Click **Attach existing network interface**.
6. Search for and select the required **Network Interface** by name.
7. Apply the changes to attach the NIC.
8. Start the virtual machine.
9. Refresh the **Network settings** page to confirm the attachment.
10. Refresh the **VM Overview** page to verify the updated configuration.

## Result
The Network Interface Card is successfully attached to the Azure Virtual Machine and active after restart.
