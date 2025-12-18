# Day 3 – Create Azure Virtual Machine Using Azure CLI

## Problem Statement
The Nautilus DevOps team is in the process of migrating some of their workloads to Azure. 
One of the tasks involves creating a new Virtual Machine (VM) using the Azure CLI. 
The team does not have access to the Azure portal but can manage Azure resources via 
the azure-client host (the landing host for this lab).

1. Create a new Azure Virtual Machine named `xfusion-vm` using the Azure CLI.
2. Use the `Ubuntu2204` image and set the VM size to `Standard_B2s`.
3. Make sure the admin username is set to `azureuser` and SSH keys are generated for secure access.
4. Use `Standard_LRS` storage account, disk size must be `30GB` and ensure the VM `xfusion-vm` is in the running state after creation.

## Objective
Create an Azure Virtual Machine using the Azure CLI with predefined compute, storage, and access settings.

## Steps
1. Open a terminal with Azure CLI installed and authenticated.
2. List all available resource groups:
   ```bash
   az group list -o table  # Displays all resource groups in the subscription in a readable table format
   ```
3. Copy the required resource group name.
4. Create the virtual machine using the following command:
   ```bash
   az vm create \
    --resource-group <resource-group-name> \
    --name <vm-name> \
    --image Ubuntu2204 \
    --size Standard_B2s \
    --admin-username <admin-username> \
    --generate-ssh-keys \
    --storage-sku Standard_LRS \
    --os-disk-size-gb 30
   ```
5. Wait for the command to complete and note the output details.

## Result
An Azure Virtual Machine is successfully created using the Azure CLI with SSH access 
and specified compute and storage configuration.
