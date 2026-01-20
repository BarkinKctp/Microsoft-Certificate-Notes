# AZ-104 – Microsoft Azure Administrator  
(microsoftlearning.github.io)

---

## Lab 1 – Manage Microsoft Entra ID Identities

<img width="3084" height="1602" alt="image" src="https://github.com/user-attachments/assets/f09af396-0ef6-4824-bea8-b9c0231ad2ca" />

A tenant is a specific instance of Microsoft Entra ID containing accounts and groups. Depending on your situation, you can create more tenants and switch between them.

Group accounts can include user accounts or devices. These are two basic ways members are assigned to groups: **statically** and **dynamically**. Static groups require administrators to add and remove members manually. Dynamic groups update automatically based on the properties of a user account or device.

**Delete resource group**
- In the Azure portal: Select the resource group → Delete the resource group → Enter resource group name → Delete  
- Azure PowerShell: `Remove-AzResourceGroup -Name resourceGroupName`  
- Azure CLI: `az group delete --name resourceGroupName`

### Extendings
- What are the Azure PowerShell and CLI commands to create a security group called IT Admins? Provide the official command reference page.  
- Provide a step-by-step strategy for managing users and groups in Microsoft Entra ID.  
- What are the steps in the Azure portal to bulk create users and groups?  
- Provide a comparison table of internal and external Microsoft Entra ID user accounts.

### Key takeaways
- A tenant represents your organization and helps you manage a specific instance of Microsoft cloud services for internal and external users.  
- Microsoft Entra ID has user and guest accounts, each with scoped access.  
- Groups combine related users or devices (Security and Microsoft 365).  
- Group membership can be static or dynamic.

---

## Lab 2a – Manage Subscription and Role-Based Access Control (RBAC)

<img width="4818" height="1347" alt="image" src="https://github.com/user-attachments/assets/b4d5b79b-82cc-40a7-9192-d33aef4b77d8" />

The root management group is built into the hierarchy so that all management groups and subscriptions roll up to it. This allows global policies and Azure role assignments at the directory level. After creating a management group, you add subscriptions that should be included.

Azure built-in roles – Azure RBAC | Microsoft Learn

Custom roles support the principle of least privilege when built-in roles grant excessive permissions.

**Clean up**
- Azure portal: Delete the resource group  
- Azure PowerShell: `Remove-AzResourceGroup -Name resourceGroupName`  
- Azure CLI: `az group delete --name resourceGroupName`

### Extendings
- Create two tables highlighting important PowerShell and CLI commands to get subscription information and explain each command.  
- What is the format of the Azure RBAC JSON file?  
- What are the basic steps for creating a custom Azure RBAC role?  
- What is the difference between Azure RBAC roles and Microsoft Entra ID roles?

### Key takeaways
- Management groups logically organize subscriptions.  
- The root management group contains all subscriptions.  
- Azure provides many built-in roles.  
- Custom roles can be created or existing ones modified.  
- Roles are defined in JSON with Actions, NotActions, and AssignableScopes.  
- Activity Log can monitor role assignments.

---

## Lab 2b – Manage Governance via Azure Policy

Policies can be assigned at the management group, subscription, or resource group level. Exclusions can also be defined.

### Extendings
- Azure PowerShell and CLI commands for adding and deleting resource locks on a resource group.  
- Table comparing Azure Policy and Azure RBAC with examples.  
- Steps to enforce Azure Policy and remediate non-compliant resources.  
- How to get a report of Azure resources with specific tags.

### Key takeaways
- Azure tags are key-value metadata.  
- Azure Policy enforces conventions.  
- Remediation tasks bring resources into compliance.  
- Resource locks prevent accidental deletion or modification.  
- Azure Policy is pre-deployment; RBAC and locks are post-deployment.

---

## Lab 3 – Manage Azure Resources Using ARM Templates

### Extendings
- What is the format of an ARM template file?  
- How to use an existing ARM template.  
- Compare ARM templates and Bicep templates.

### Key takeaways
- ARM templates deploy, manage, and monitor resources as a group.  
- ARM templates are JSON files.  
- Templates can be deployed via portal, PowerShell, or CLI.  
- Bicep provides concise syntax and type safety.

---

## Lab 4 – Implement Virtual Network

**Scenario**
- CoreServicesVnet requires a large address space.  
- ManufacturingVnet supports internal connected devices.

### Extendings
- Best practices for deploying VNets.  
- PowerShell and CLI commands to create a VNet.  
- Explain NSG inbound and outbound rules.  
- Difference between NSGs and ASGs.  
- Network troubleshooting steps.

### Key takeaways
- VNets represent networks in the cloud.  
- Avoid overlapping IP ranges.  
- Subnets organize and secure networks.  
- NSGs control traffic.  
- Azure DNS resolves names.

---

## Lab 5 – Implement Intersite Connectivity

### Extendings
- PowerShell or CLI commands for VNet peering.  
- Azure and third-party monitoring tools.  
- When to create custom routes.

### Key takeaways
- VNets are isolated by default.  
- VNet peering connects networks.  
- Peered VNets use the Microsoft backbone.  
- Network Watcher monitors connectivity.

---

## Lab 6 – Implement Traffic Management

### Extendings
- Compare Azure Load Balancer and Application Gateway.  
- Troubleshoot inbound connectivity.  
- Configure Application Gateway.  
- Table comparing Azure load-balancing solutions.

### Key takeaways
- Azure Load Balancer operates at OSI layer 4.  
- Application Gateway operates at OSI layer 7.  
- Standard Load Balancer offers high performance.  
- Application Gateway supports WAF and routing rules.

---

## Lab 7 – Manage Azure Storage

### Extendings
- PowerShell script to create storage.  
- Storage security checklist.  
- Storage redundancy comparison table.

### Key takeaways
- Storage accounts support blobs, files, queues, and tables.  
- Redundancy options include LRS, ZRS, and GRS.  
- Blob storage handles unstructured data.  
- File storage supports shared structured data.  
- Immutable storage supports WORM.

---

## Lab 8 – Manage Virtual Machines

### Extendings
- Azure CLI steps to create a Linux VM.  
- VM scaling options.  
- Storage lifecycle management.

### Key takeaways
- Azure VMs provide scalable compute.  
- Vertical and horizontal scaling are supported.  
- VM Scale Sets manage groups of VMs.  
- Autoscaling is supported.

---

## Lab 9a – Implement Web Apps

### Extendings
- Steps to create and configure a web app.  
- Ways to scale a web app.

### Key takeaways
- Azure App Service hosts web apps.  
- Multiple runtimes are supported.  
- Deployment slots enable testing.  
- Scaling can be manual or automatic.

---

## Lab 9b – Implement Azure Container Instances

### Extendings
- Steps to create an Azure Container Instance.  
- Ways to run serverless containers.

### Key takeaways
- ACI runs containers without infrastructure management.  
- Linux and Windows containers are supported.  
- Workloads are typically short-lived.

---

## Lab 9c – Implement Azure Container Apps

### Extendings
- Steps to create an Azure Container App.  
- Compare Azure Container Apps and AKS.

### Key takeaways
- Azure Container Apps is a serverless container platform.  
- Orchestration and deployment are managed.  
- Workloads are usually long-running.
