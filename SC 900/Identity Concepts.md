# Identity Concepts

- **Authentication**: Verifies who a user is.
- **Authorization**: Determines what an authenticated user can access.

---

## Identity Pillars
- Administration  
- Authentication  
- Authorization  
- Auditing  

- **Administration**: Managing user accounts.
- **Authentication**: Identifying who the user is.
- **Authorization**: Defining access levels for users.
- **Auditing**: Tracking authentication, authorization, administration, and access activities.

---

## Identity Provider
A system that creates, maintains, and manages identity information.

---

## Single Sign-On (SSO)
- Allows access to multiple applications with one sign-in.
- Uses **federation** to trust external identity providers.

---

## Active Directory
- **Active Directory (AD)**
- **Active Directory Domain Services (AD DS)**

---

## Microsoft Entra ID – Authentication

### Authentication Methods

#### Password Authentication
- Passwords

#### Phone Authentication
- SMS-based authentication  
- Voice call verification  

#### OATH (Open Authentication)
- Software OATH tokens  
- OATH TOTP (time-based one-time password) hardware tokens  

#### Passwordless Authentication
- FIDO2 (Fast Identity Online)  
- Windows Hello  
- Microsoft Authenticator App  

#### Certificate-Based Authentication

#### Primary and Secondary Authentication

---

## Multifactor Authentication (MFA)
Uses two or more of the following:
- Something you know (password or PIN)
- Something you have (phone, hardware key)
- Something you are (biometrics such as fingerprint or face scan)

---

## Self-Service Password Reset (SSPR)

---

## Password Protection and Management
- Global banned password list  
- Custom banned password lists  
- Password spray protection  
- Hybrid security  

---

## Key Notes

- OATH hardware tokens use time-based one-time passwords.
- Strong passwords are not one-time passwords.
- Password hash synchronization syncs password hashes between Active Directory and Microsoft Entra tenant.
- Windows Hello uses a camera or passcode for authentication.

---

## Hybrid Identity

An organization migrating to the Microsoft cloud with a hybrid identity model can use:
- **Microsoft Entra Connect** to sync identities between AD DS and Microsoft Entra ID.

Not suitable:
- AD FS (not used for hybrid identity sync)
- Microsoft Sentinel (security monitoring, not identity)
- PIM (used for privileged access management)

---

## Authentication vs Authorization
- Authentication: Identifies the user.
- Authorization: Determines access level.
- Administration: Manages accounts.
- Auditing: Tracks all identity-related activities.

---

## Strongest Authentication Method
- Microsoft Authenticator app (phone sign-in)  
Enforcing password changes or complexity alone is not sufficient.  
Soft tokens are weaker than Microsoft Authenticator.

---

## Managed Identities and App Identities

- **Managed identities**: Fully managed by Microsoft Entra, used by Azure resources to access other Azure resources.
- **Service principal**: Identity for an application.
  - Applications must be registered in Microsoft Entra.
  - A service principal is created per tenant where the app is used.
- **Device identity**: Used for devices, not for accessing Azure resources directly.
- **User identity**: Requires manual password management.

---

## Microsoft Entra ID Licensing

- Monthly Active Users (MAU) billing applies to all tenants.
- Microsoft Entra ID P1 and P2 do not charge for the first 50,000 MAU.
- P1 is the minimum edition that supports MAU benefits.
- Free and Microsoft Entra External ID charge per user and do not provide the 50,000 MAU benefit.
- Microsoft Entra ID P2 includes entitlement management (access packages).

---

## Microsoft Entra ID vs Active Directory
- Microsoft Entra ID does not require domain controller servers.
- Active Directory requires physical or virtual servers.
- Google and Facebook identities require federation.
