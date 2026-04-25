
# Three Tier VMSS Application Deployent 

This model provisions a three tier application using VM Scale Sets and a private database to deploy a flask app gunicorn server on an Ubuntu instance.

---

## 🌐 Live Project Links

- 🔴 RedHat Infrastructure Overview:  
  https://www.fejzic37.com/links/vmbased_azure.html

---

## ⚙️ What this project does

- Provisions a full 3-tier Azure architecture using Terraform
- Deploys a VM Scale Set (VMSS) as the application tier
- Configures a private database tier isolated from public access
- Automates infrastructure using Terraform

---

## 🧱 Tech Stack

- Azure Cloud (VNet, VMSS, Bastion, Load Balancer, VM instances)
- Linux VMs (Application Tier)
- Python / Flask or application runtime
- Azure Database (MySQL/PostgreSQL depending on configuration)

### ☁️ Cloud & Infrastructure
- Azure VM Scale Sets (auto-scaling application tier)
- Azure Load Balancer for distributing traffic to VMSS
- Network Security Groups (NSGs) for layered access control

### 💻 Application Layer
- Gubicorn / Flask HTTP Server
- VM Scale Set running application instances

### 🗄️ Database
- MySQL
- Relational schema for application data storage
- Replica database

### 🔐 Security
- Bastion Host
- NSG rules restricting inbound/outbound traffic
- Secure internal-only database communication

### 📊 Observability
- Log Analytics Workspace
- Collection rules from all subnets


Architecture Diagram

<img width="1048" height="1070" alt="image" src="https://github.com/user-attachments/assets/4c6237dc-1626-4ba5-a7e9-e9b00b60101d" />
