# Day 15 – Create and Configure Network Security Group (NSG) in Azure

## Problem Statement
The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the Azure cloud. Recognizing the scale 
of this undertaking, they have opted to approach the migration in incremental steps rather than as a single massive transition. 
To achieve this, they have segmented large tasks into smaller, more manageable units. This granular approach enables the team to execute the migration 
in gradual phases, ensuring smoother implementation and minimizing disruption to ongoing operations. By breaking down the migration into smaller tasks, 
the Nautilus DevOps team can systematically progress through each stage, allowing for better control, risk mitigation, 
and optimization of resources throughout the migration process.

For this task, create a network security group (NSG) with the following requirements:
- Name of the NSG should be `datacenter-nsg`.
- Add an inbound security rule named `Allow-HTTP` for HTTP service on `port 80`, with the source CIDR range of `0.0.0.0/0`.
- Add another inbound security rule named `Allow-SSH` for SSH service on `port 22`, with the source CIDR range of `0.0.0.0/0`.

## Objective
Create a Network Security Group and configure inbound security rules to control traffic to Azure resources.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Network Security Groups** and open the service.
3. Click **Create**.
4. Configure the **Basics** tab:
   - Enter an **NSG name**.
   - Select or create a **Resource Group**.
5. Click **Review + Create**.
6. Click **Create**, then select **Go to resource**.
7. In the NSG menu, navigate to **Settings** → **Inbound security rules**.
8. Click **Add**.
9. Configure the inbound rule:
   - Enter a **Rule name**.
   - Set **Source** to *Any*.
   - Enter the required **Source port range**.
   - Choose the appropriate **Service**.
10. Click **Save**.
11. Repeat the process to add additional inbound security rules as required.

## Result
A Network Security Group is successfully created with inbound security rules applied to control network access.
