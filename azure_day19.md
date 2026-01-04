# Day 19 – Convert Public Azure Blob Container to Private

## Problem Statement
The Nautilus DevOps team has been using Azure Blob Storage to manage their data. Recently, they realized that one of their containers, 
currently public, needs to be restricted for internal use only. Your task is to convert a public Azure Blob container to private.

Two blob containers named `datacenter-container-15409` and `datacenter-priv-11827` are available in the `East US` region 
within the storage account `datacenterst5467`. The `datacenter-container-15409` is currently public, and `datacenter-priv-11827` is private.

1. Convert the blob container `datacenter-container-15409` from public to private while leaving `datacenter-priv-11827` unchanged.
2. Make sure the access level for `datacenter-container-15409` is set to private with no public access.

## Objective
Change an Azure Blob Storage container’s access level from public to private.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Search for and open the target **Storage account**.
3. Navigate to **Storage browser** → **Blob containers**.
4. Select the **Public Blob container**.
5. Click **Change access level**.
6. Set the access level to **Private**.
7. Click **OK** to apply the change.
8. Refresh the **Blob containers** page to verify the update.

## Result
The Azure Blob Storage container is successfully converted from public to private, restricting anonymous access.
