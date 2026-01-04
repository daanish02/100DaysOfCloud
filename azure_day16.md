# Day 16 – Create a Private Azure Blob Storage Container

## Problem Statement
As part of the data migration process, the Nautilus DevOps team is actively creating several storage containers on Azure. 
They plan to utilize private Blob containers to store the relevant data. Given the ongoing migration of other infrastructure to Azure, 
it is logical to consolidate data storage within the Azure environment as well.

- Create a new storage account named `datacenterst17723` and a private Blob container named `datacenter-blob-9913` within the storage account.

## Objective
Create a private Azure Blob Storage container for secure object storage.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, search for **Storage accounts** (Storage center) and open the service.
3. Click **Create**.
4. Configure the **Basics** tab:
   - Enter a **Storage account name**.
   - Select or create a **Resource Group**.
   - Choose the preferred **Storage type**:
     - Azure Blob Storage, or
     - Azure Data Lake Storage Gen2.
5. Click **Review + Create**.
6. Click **Create**, then select **Go to resource**.
7. Navigate to **Storage browser** → **Blob containers**.
8. Click **Add container**.
9. Enter the **Container name**.
10. Click **Create**.

## Result
A private Azure Blob Storage container is successfully created and ready to store data securely.
