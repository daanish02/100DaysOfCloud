# Day 11 – Change Azure Virtual Machine Size Using Console

## Problem Statement
The Nautilus DevOps team is migrating a portion of their infrastructure to 
Azure. During the migration, they have created several virtual machines
 (VMs) in different regions. The team has identified one VM 
that is underutilized and has decided to change its size 
to optimize resource usage.

- Change the VM size from `Standard_B1s` to `Standard_B2s` for the 
virtual machine named `xfusion-vm`.
- Ensure the VM is in the running state after the size change is complete.

## Objective
Resize an Azure Virtual Machine to modify its compute capacity using the Azure portal.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open the target **Virtual Machine**.
3. Stop the virtual machine.  
   > A VM must be stopped before resizing.
4. In the VM menu, navigate to **Availability + scale** → **Size**.
5. Select the required **Virtual Machine size**.
6. Click **Resize** to apply the new configuration.
7. Navigate to the virtual machine **Overview** page.
8. Start the virtual machine.

## Result
The Azure Virtual Machine is successfully resized and running with the updated compute resources.
