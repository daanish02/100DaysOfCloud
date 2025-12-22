# Day 7 – Create a Public IP Address for Azure VM

## Problem Statmement
The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the Azure cloud. 
Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than 
as a single massive transition. To achieve this, they have segmented large tasks into smaller, more manageable units. 
This granular approach enables the team to execute the migration in gradual phases, ensuring smoother implementation and 
minimizing disruption to ongoing operations. By breaking down the migration into smaller tasks, the Nautilus DevOps team can 
systematically progress through each stage, allowing for better control, risk mitigation, and optimization of resources 
throughout the migration process.

For this task, allocate a `Public IP` address, name it as `xfusion-pip`.

## Objective
Create a public IP address resource in Azure for enabling external connectivity to a virtual machine.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Public IP addresses** and open the service.
3. Click **Create**.
4. Configure the **Basics** tab:
   - Select or create a **Resource Group**.
   - Enter a **Public IP name**.
5. Skip the remaining configuration steps.
6. Click **Review + Create**.
7. Click **Create** to deploy the public IP address.

## Result
A public IP address resource is successfully created and ready to be associated with an Azure virtual machine.
