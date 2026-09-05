# Azure-Enterprise-Architecture-Lab
# Project 1: Secure Hub and Spoke Network Architecture in Azure

## 📖 Project Overview
In enterprise cloud environments, security and centralized network management are critical. For this project, I designed and deployed a Hub and Spoke network topology in Microsoft Azure. This architecture isolates production and development workloads into separate "Spoke" networks, while routing all administrative access through a centralized, highly secure "Hub" network using Azure Bastion.

## 🛠️ Skills & Technologies Demonstrated
* Azure Virtual Networks (VNet)
* VNet Peering & Routing
* Azure Bastion (Secure RDP/SSH)
* Network Security Groups (NSGs)
* Private IP Addressing

## 🚀 Step-by-Step Implementation

### Step 1: Resource Group Deployment
I provisioned a dedicated resource group to contain the entire network infrastructure, including the Hub VNet, two Spoke VNets (Prod and Dev), and the Bastion host.

![Resource Group Overview](./Screenshot_123631.png)

### Step 2: Network Topology Design
Using Azure Network Watcher, I validated the visual topology of the environment. The `Hub_Vnet` acts as the central point of connectivity for both `Spoke1_prod` and `Spoke2_dev`.

![Network Topology](./Screenshot_123106.png)

### Step 3: Configuring VNet Peering
To allow the Hub to communicate with the isolated Spokes, I configured bidirectional VNet peering. This allows seamless internal traffic routing across the Azure backbone without exposing data to the public internet.

![VNet Peerings](./Screenshot_123231.png)

### Step 4: Securing the Workload VM
I deployed an Ubuntu virtual machine (`VmSpokeProd`) into the production spoke. To ensure maximum security, I did not attach a Public IP address. The VM is only accessible internally via its private IP (`10.1.1.4`) and is protected by a strict Network Security Group (NSG).

![VM Network Settings](./Screenshot_123519.png)

### Step 5: Implementing Azure Bastion
Because the VM has no public IP, traditional SSH over the internet is impossible. I deployed Azure Bastion in the Hub network to securely bridge the gap.

![Bastion Connection](./Screenshot_122655.png)

### Step 6: Successful Secure Connection
Using Bastion, I successfully established a secure SSH session into the isolated Spoke VM directly through the Azure Portal, proving the architecture works exactly as intended.

![Ubuntu CLI via Bastion](./Screenshot_122442.png)

## 💡 Key Takeaways
This project demonstrated how to build a scalable, enterprise-grade network foundation. By utilizing a Hub and Spoke model with Azure Bastion, I successfully eliminated the need for exposed public IP addresses and open management ports, drastically reducing the environment's attack surface.
