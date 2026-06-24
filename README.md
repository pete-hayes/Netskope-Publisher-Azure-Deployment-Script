# Netskope Publisher Azure Deployment Script
A lightweight `cloud-init` configuration that enables zero-touch registration for Netskope Private Access Publishers in Microsoft Azure. By pasting this script into Azure's Custom data field at launch, the instance automatically verifies basic outbound connectivity and registers itself with your Netskope tenant, eliminating the need to assign a public IP or manually SSH into the box.

## Usage
1. Follow Netskope's [instructions](https://docs.netskope.com/en/create-a-new-publisher#configure-a-publisher-in-azure) for deploying the Publisher within Azure, but pause before creating the virtual machine
2. Navigate to the **Advanced** section
3. Copy the contents of [azure-publisher-custom-data.yaml](azure-publisher-custom-data.yaml) into the **Custom data** field
4. Replace `<token>` with a Netskope Publisher token generated within your Netskope Administrator Portal
5. Complete the remaining steps per Netskope's documentation and click **Create**

<p align="center">
<img width="50%" height="50%" alt="Publisher-Deployment-Script" src="https://github.com/user-attachments/assets/00056fb0-e19a-4099-abcd-a326c6fe6509" />
</p>

## License
Licensed under MIT — free to use, modify, and share, with no warranty.

## Disclaimer
This project is **not affiliated with or supported by Netskope**. It may be incomplete, outdated, or inaccurate. Use at your own risk. 
