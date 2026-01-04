# Day 20 – Backup and Delete Azure Storage Blob Container

## Problem Statement
The Nautilus DevOps team is currently engaged in a cleanup process, focusing on removing unnecessary data and services 
from their Azure environment. As part of the migration process, several resources were created for one-time use only, 
necessitating a cleanup effort to optimize their Azure environment.

A private blob container named `devops-blob-23538` already exists in the `East US` region under storage account `devopsst20331`.

1. Copy the contents of `devops-blob-23538` blob container to the `/opt` directory on the azure-client host (the landing host once you load this lab).
2. Delete the blob container `devops-blob-23538` from the storage account.

## Objective
Back up data from an Azure Blob Storage container and delete the container using Azure CLI.

## Steps

1. Log in to the Azure client host machine.
2. Ensure Azure CLI is installed and authenticated.
3. Download all blobs from the container to a local directory:
   ```bash
   sudo az storage blob download-batch \
       --destination /opt \
       --source <container-name> \
       --account-name <storage-account-name> \
       --auth-mode login
   ```
4. Delete the Blob Storage container:
   ```bash
   az storage container delete \
    --name <container-name> \
    --account-name <storage-account-name> \
    --auth-mode login
   ```

## Result
Blob data is successfully backed up locally, and the Azure Blob Storage container is deleted.
