# Day 17 – Create a Public Azure Blob Storage Container

## Problem Statement
As part of the data migration process, the Nautilus DevOps team is actively creating several storage containers on Azure. They plan 
to utilize public Blob containers to store the relevant data. Given the ongoing migration of other infrastructure to Azure, 
it is logical to consolidate data storage within the Azure environment as well.

- Create a new storage account named `devopsst13050` and a public Blob container named `devops-blob-23124` within the storage account. 
Make sure anonymous read access for containers and blobs is enabled.

## Objective
Create a public Azure Blob Storage container with anonymous read access enabled.

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
5. Navigate to **Advanced** → **Security**.
6. Enable **Anonymous read access for containers and blobs**.
7. Click **Review + Create**.
8. Click **Create**, then select **Go to resource**.
9. Navigate to **Storage browser** → **Blob containers**.
10. Click **Add container**.
11. Enter the **Container name**.
12. Set **Anonymous access level** to **Container**.
13. Click **Create**.

## Result
A public Azure Blob Storage container is successfully created with anonymous read access enabled.
