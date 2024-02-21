# SSH into Debian Linux VMs Using PuTTY

This guide provides step-by-step instructions for accessing Magento VMs (`magento1` and `magento2`) from a Windows system using PuTTY, utilizing the `magento.ppk` private key for authentication. The login user for both VMs is `magento`.

## Prerequisites

- PuTTY installed on your Windows machine. If not installed, download it from [PuTTY download page](https://www.putty.org/).
- Access to the `magento.ppk` private key file.

## Instructions

### 1. Launch PuTTY

Open the PuTTY SSH client on your Windows device.

### 2. Session Configuration

In the "Host Name (or IP address)" field, type the hostname or IP address of the VM:

- For Magento1 VM: `server1.pawtech.com.au` (Port `22`)
- For Magento2 VM: `server2.pawtech.com.au` (Port `2222`)

### 3. Configure Private Key

- In the Category pane, navigate to `Connection > SSH > Auth`.
- Click "Browse" next to "Private key file for authentication" and select the `magento.ppk` file.

### 4. Enter User Name

- Before opening the connection, return to the "Session" page.
- In the "Auto-login username" field under "Connection > Data", enter `magento`.

### 5. Save Session (Optional)

- On the "Session" category, type a name for this session (e.g., `Magento1` or `Magento2`) in the "Saved Sessions" field.
- Click "Save" for future convenience.

### 6. Open Connection

- Click "Open" to initiate the SSH connection.
- If prompted about the server's host key, select "Yes" to acknowledge and proceed.

You are now connected to your Magento VM via SSH using PuTTY, with no password prompt due to the key-based authentication setup.

## Repeat the Process

To connect to each VM, repeat these steps, ensuring the correct hostname and port are used.
