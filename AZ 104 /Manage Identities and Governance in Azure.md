MICROSOFT ENTRA ID
-Azure AD DS and MS Entra ID
AD DS is a directory service that provides the methods for storing directory data, such as user accounts and passwords, and makes this data available to network users, administrators, and other devices and services. It runs as a service on Windows Server, referred to as a domain controller.
Microsoft Entra ID is part of the platform as a service (PaaS) offering and operates as a Microsoft-managed directory service in the cloud. 
With Microsoft Entra ID, you also have access to a set of features that aren’t natively available in AD DS, such as support for multi-factor authentication, identity protection, and self-service password reset.

<img width="2145" height="900" alt="image" src="https://github.com/user-attachments/assets/4aa12c47-d81a-4a16-aa08-88713cf73f60" />

By default, when you create a new Azure subscription by using a Microsoft account, the subscription automatically includes a new Microsoft Entra tenant named Default Directory.

Entra Tenants
Unlike AD DS, Microsoft Entra ID is multi-tenant by design and is implemented specifically to ensure isolation between its individual directory instances. 
At any given time, an Azure subscription must be associated with one, and only one, Microsoft Entra tenant. This association allows you to grant permissions to resources in the Azure subscription (via RBAC) to users, groups, and applications that exist in that particular Microsoft Entra tenant.
You can associate the same Microsoft Entra tenant with multiple Azure subscriptions. This allows you to use the same users, groups, and applications to manage resources across multiple Azure subscriptions.
Each Microsoft Entra tenant is assigned the default Domain Name System (DNS) domain name, consisting of a unique prefix. The prefix, derived from the name of the Microsoft account you use to create an Azure subscription or provided explicitly when creating a Microsoft Entra tenant, is followed by the onmicrosoft.com suffix. Adding at least one custom domain name to the same Microsoft Entra tenant is possible and common. 

Entra Schema
The Microsoft Entra schema contains fewer object types than that of AD DS. Most notably, it doesn't include a definition of the computer class, although it does include the device class. The process of joining devices to Microsoft Entra differs considerably from the process of joining computers to AD DS. The Microsoft Entra schema is also easily extensible, and its extensions are fully reversible.


-Compare Microsoft Entra ID and Active Directory Domain Services
AD DS is the traditional deployment of Windows Server-based Active Directory on a physical or virtual server. 
--Active Directory Certification Services (AD CS)
--Active Directory Lightweight Directory Services (AD LDS)
--Active Directory Federation Services (AD FS)
--Active Directory Rights Management Services (AD RMS)

s
<img width="2145" height="900" alt="image" src="https://github.com/user-attachments/assets/bfeb8b6b-f4df-4f74-a249-9e95ea3b69b3" />
