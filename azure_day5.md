# Day 5 – Create a Virtual Network (IPv4) in Azure

## Problem Statement
The Nautilus DevOps team is strategically planning the migration of a portion of their infrastructure to the Azure cloud. 
Acknowledging the magnitude of this endeavor, they have chosen to tackle the migration incrementally rather than as a single, 
massive transition. Their approach involves creating Virtual Networks (VNets) as the initial step, as they will be provisioning 
various services under different VNets.

- Create a Virtual Network (VNet) named `xfusion-vnet` in the `East US` region with `192.168.0.0/24` IPv4 CIDR.

## Objective
Create an Azure Virtual Network with a custom IPv4 address space.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Virtual Networks** and open the service.
3. Click **Create**.
4. Configure the **Basics** tab:
   - Select or create a **Resource Group**.
   - Enter a **Virtual Network name**.
   - Choose the **Region**.
5. Navigate to the **IP Addresses** tab.
6. Under **IPv4 address space**, enter the required address range with prefix (CIDR notation).
7. Skip the remaining configuration steps.
8. Click **Review + Create**.
9. Click **Create** to deploy the virtual network.

## Result
A Virtual Network with a defined IPv4 address space is successfully created in Azure.
