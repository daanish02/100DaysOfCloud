# Day 4 – Create a Virtual Network (VNet) in Azure

## Problem Statement
The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the Azure cloud. 
Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than 
as a single massive transition. To achieve this, they have segmented large tasks into smaller, more manageable units. 
This granular approach enables the team to execute the migration in gradual phases, ensuring smoother implementation 
and minimizing disruption to ongoing operations.

- Create a Virtual Network (VNet) named `nautilus-vnet` in the `East US` region with any IPv4 CIDR block.

## Objective
Create an Azure Virtual Network to provide isolated networking for cloud resources.


## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Virtual Networks** and open the service.
3. Click **Create**.
4. Configure the **Basics** tab:
   - Select or create a **Resource Group**.
   - Enter a **Virtual Network name**.
   - Choose the **Region**.
5. Skip the remaining configuration steps.
6. Click **Review + Create**.
7. Click **Create** to deploy the virtual network.

## Result
A Virtual Network is successfully created and ready to be used for deploying and connecting Azure resources.
