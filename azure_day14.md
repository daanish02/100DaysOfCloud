# Day 14 – Create and Attach Managed Disks in Azure

## Problem Statement
The Nautilus DevOps team is strategizing the migration of a portion 
of their infrastructure to the Azure cloud. Recognizing the scale 
of this undertaking, they have opted to approach the migration 
in incremental steps rather than as a single massive transition. 
To achieve this, they have segmented large tasks into smaller, 
more manageable units. This granular approach enables the team to execute 
the migration in gradual phases, ensuring smoother implementation 
and minimizing disruption to ongoing operations. By breaking down 
the migration into smaller tasks, the Nautilus DevOps team 
can systematically progress through each stage, allowing 
for better control, risk mitigation, and optimization of resources 
throughout the migration process.

Create a managed disk with the following requirements:
- Name of the disk should be `nautilus-disk`.
- Disk type must be `Standard_LRS`.
- Disk size must be `2 GiB`.

## Objective
Create a managed disk in Azure and prepare it for attachment to a virtual machine.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Disks** and open the service.
3. Click **Create**.
4. Configure the **Basics** tab:
   - Enter a **Disk name**.
   - Select or create a **Resource Group**.
5. Under **Disk size**:
   - Select **Standard HDD (LRS)**.
   - Specify the required **Disk size**.
6. Click **Review + Create**.
7. Click **Create** to deploy the managed disk.

## Result
A managed disk is successfully created in Azure and is ready 
to be attached to a virtual machine.
