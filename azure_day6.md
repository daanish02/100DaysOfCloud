# Day 6 – Create a Subnet in Azure Virtual Network

## Problem Statement
The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the Azure cloud. 
Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps rather than 
as a single massive transition.

- For this task, create a Virtual Network (VNet) named `xfusion-vnet` and one subnet named `xfusion-subnet` 
within the VNet in the `East US` region. Make sure the IPv4 address range is `10.0.0.0/16`.

## Objective
Create a subnet within an Azure Virtual Network to logically segment network resources.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Virtual Networks** and open the service.
3. Click **Create**.
4. Configure the **Basics** tab:
   - Select or create a **Resource Group**.
   - Enter a **Virtual Network name**.
   - Choose the **Region**.
5. Navigate to the **IP Addresses** tab.
6. Under **IPv4 address space**, click **Add subnet**.
7. Enter the **Subnet name**.
8. Select the **IPv4 address range** by specifying the starting address and subnet size.
9. Skip the remaining configuration steps.
10. Click **Review + Create**.
11. Click **Create** to deploy the virtual network with the subnet.

## Result
A subnet is successfully created within the Azure Virtual Network, enabling structured network segmentation.
