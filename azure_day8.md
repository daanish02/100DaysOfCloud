# Day 8 – Attach Managed Disk to Azure Virtual Machine

## Problem Statement
The Nautilus DevOps team is migrating services to Azure. 
They are breaking down tasks to ensure better control and 
optimization. You are tasked with attaching an existing 
data disk to a virtual machine (VM).

An existing VM named `devops-vm` and a managed disk 
named `devops-disk` already exist in the East US region.

- Attach the disk devops-disk to the VM devops-vm as a data disk.
- Ensure the disk is attached to the VM devops-vm.
- Make sure that the virtual machine initialization has been 
completed before submitting this task.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open the target **Virtual Machine**.
3. In the VM menu, navigate to **Settings** → **Disks**.
4. Click **Attach existing disks**.
5. Search for and select the required **Managed Disk** by name.
6. Apply the changes to attach the disk.
7. Refresh the **Disks** page to confirm the attachment.
8. Refresh the **VM Overview** page to verify the updated configuration.

## Result
The managed disk is successfully attached to the Azure Virtual Machine and is available for use.
