# Day 1 – Create SSH Key Pair for Azure Virtual Machine

## Problem Statement
The Nautilus DevOps team is strategizing the migration of a portion of their infrastructure to the Azure cloud. 
Recognizing the scale of this undertaking, they have opted to approach the migration in incremental steps 
rather than as a single massive transition. To achieve this, they have segmented large tasks into 
smaller, more manageable units. This granular approach enables the team to execute the migration in gradual phases, 
ensuring smoother implementation and minimizing disruption to ongoing operations. By breaking down the migration 
into smaller tasks, the Nautilus DevOps team can systematically progress through each stage, allowing for 
better control, risk mitigation, and optimization of resources throughout the migration process.

For this task, create an SSH key pair with the following requirements:
- The name of the SSH key pair should be datacenter-kp.
- The key pair type must be rsa.

## Objective
Create an SSH key pair in Azure for secure, passwordless access to virtual machines.

## Steps

1. Log in to the Azure Portal using your credentials.
2. In the search bar, type **SSH keys** and open the service.
3. Click **Create**.
4. Select or create a **Resource Group**.
5. Enter a **Key pair name**.
6. Choose **Generate key pair**.
7. Select the required **Key pair type**.
8. Skip the optional configuration steps.
9. Click **Create**.
10. Download and securely store the private key on your local machine.

## Result
An SSH key pair is successfully created and ready to be used for authenticating Azure virtual machines.

