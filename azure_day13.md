# Day 13 – SSH into an Azure Virtual Machine

## Problem Statement
The Nautilus DevOps team is working on setting up secure SSH access for their virtual machines in Azure. One of the requirements is to add the SSH public key of the root user 
from the Azure client host (landing host) to the `xfusion-vm` Azure VM's `authorized_keys` file. This ensures secure and password-less SSH access to the VM.

Task Details:
- VM Details: The VM is named `xfusion-vm` and is running in the `West US` region. The default SSH user is `azureuser` — use this user to connect to the VM. You need to add the root user's SSH public key 
from the Azure client host to the authorized_keys file of the VM's root user. The SSH public key of the root user on the Azure client host is located at `/root/.ssh/id_rsa.pub`.
- Public Key Addition: Copy the public key located at `/root/.ssh/id_rsa.pub` on the Azure client host to the authorized_keys file of the root user on `xfusion-vm`. Ensure that the 
proper permissions for the `.ssh` folder and `authorized_keys` file are set on the VM.
- Verification: After adding the public key, make sure that you are able to SSH into the `xfusion-vm` VM as the root user from the Azure client host without needing a password.

**Important Notes**:
Ensure that the VM is up and running before attempting to SSH.  
You may need to adjust the firewall or security group rules for the VM to allow SSH access.

## Objective
Access an Azure Virtual Machine using SSH and configure key-based access for the root user.

## Steps

1. Log in to the Azure Portal using your credentials.
2. Open the target **Virtual Machine** and note the **Public IP address** from the overview.
3. On the Azure client host terminal, navigate to the SSH directory:
   ```bash
   cd ~/.ssh
   ```
4. Copy the SSH public key.
5. SSH into the Azure virtual machine:
   ```bash
   ssh <username>@<public-ip-address>
   ```
6. Gain root access:

   ```bash
   sudo -i
   ```
7. Navigate to the root SSH directory:
   ```bash
   cd /root/.ssh
   ```
8. Paste the copied public key into the appropriate authorized keys file.
9. Exit the SSH session.
10. Verify root access by reconnecting:
   ```bash
   ssh root@<public-ip-address>
   ```

## Result
SSH access to the Azure Virtual Machine is successfully configured and verified for the root user.
