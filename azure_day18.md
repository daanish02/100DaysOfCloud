# Day 18 – Copy Data to an Azure Blob Storage Container

## Problem Statement
The Nautilus DevOps team is presently immersed in data migrations, transferring data from on-premise storage systems to Azure Blob containers. 
They have recently received some data that they intend to copy to one of the Blob containers.

- A Blob container named `nautilus-blob-28911` already exists in the `East US` region under the storage account `nautilusst18364`. 
- Copy the file `/tmp/nautilus.txt` to the Blob container `nautilus-blob-28911`.

## Objective
Upload data to an Azure Blob Storage container using the Azure Portal.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open the target **Storage account**.
3. Navigate to **Storage browser** → **Blob containers**.
4. Select the required **Blob container**.
5. Click **Upload**.
6. Choose the file to upload.
7. Click **Upload** to start the data transfer.

## Result
Data is successfully uploaded to the Azure Blob Storage container and available for access based on the configured permissions.
