# azure-linux-vm-iac
An Azure Linux VM deployment using Terraform (IaC). Includes resource group, virtual network, subnet, and a Linux VM with SSH access.

# Azure Linux VM with Terraform

This repository demonstrates Infrastructure as Code (IaC) for deploying a Linux VM in Azure using Terraform. It covers:

- Creating a resource group
- Setting up a virtual network and subnet
- Deploying a Linux VM with SSH access
- Using Terraform modules and best practices

---

## Architecture

Internet → Public IP → NIC → VM in Subnet → VNet → Resource Group


---

## Prerequisites

- Azure account (free trial or subscription)
- Terraform CLI (v1.5+)
- Azure CLI
- SSH key pair

---

## Usage

1. Clone the repository:

git clone https://github.com/yourusername/azure-linux-vm-iac.git
cd azure-linux-vm-iac


2. Log in to Azure:
az login


3. Initialize Terraform:
terrafrom init


4. Plan and apply:
terraform plan
terraform apply


5. SSH into the VM:
ssh azureuser@<vm_public_ip>


---

## Repository Structure

- `main.tf`: Main Terraform configuration
- `variables.tf`: Input variables
- `outputs.tf`: Output values

---

## Customization

- Change the region by updating the `location` variable.
- Adjust VM size by modifying the `size` parameter.
- Customize the Linux image by updating the `source_image_reference`.

---

## License

MIT


