# Azure ID, Access, Security

## Conditional Access
Conditional Access is a feature that Microsoft Entra uses to allow or deny access to resources based on identity signals, such as the device being used.  
Conditional Access allows administrators to control, allow, or deny access to resources based on certain signals.  
You can require that access to certain applications only be allowed if the users are using an approved client application.  
Conditional Access can use signals to determine information about authentication attempts, and then determine whether to block access or require additional verifications, such as MFA.

---

## Single Sign-On (SSO)
SSO enables a user to sign in one time and use that credential to access multiple resources and applications from different providers.

---

## Multi-Factor Authentication (MFA)
MFA is a process whereby a user is prompted during the sign-in process for an additional form of identification.  
Examples include a code on their mobile phone or a fingerprint scan.

---

## Hybrid Identity
Hybrid identity solutions create a common user identity for authentication and authorization to all resources, regardless of location.

---

## Azure RBAC
An Azure RBAC role is applied to a scope, which is a resource or set of resources that the access applies to.  
Resource locks prevent the accidental change or deletion of a resource.  
Resource tags are used to locate and act on resources associated with specific workloads, environments, business units, and owners.  
Policies enforce different rules across resource configurations so that the configurations stay compliant with corporate standards.

---

## Defense in Depth
A defense in depth strategy uses a series of mechanisms to slow the advancement of an attack that aims to gain unauthorized access to data.  
The principle of least privilege means restricting access to information to only the level that users need to perform their work.  
A DDoS attack attempts to overwhelm and exhaust an application's resources.  
The perimeter layer is about protecting an organization's resources from network-based attacks.

---

## Microsoft Entra Connect
Microsoft Entra Connect syncs user identities from an on-premises Active Directory Domain Services (AD DS) domain to Microsoft Entra.  
Microsoft Entra Connect allows you to use features such as single sign-on (SSO), MFA, and self-service password reset (SSPR) in both systems.  
SSPR prevents users from using known compromised passwords.
