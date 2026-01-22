## Microsoft Entra ID Protection and Governance

### Microsoft Entra ID Governance

#### Identity Lifecycle
Manages how identities are created, updated, and removed.

#### Access Lifecycle
Controls how users gain, maintain, and lose access to resources.

#### Privileged Access Lifecycle
Managed using **Microsoft Entra Privileged Identity Management (PIM)**.

---

## Access Reviews
Used to ensure appropriate access over time:
- Too many users in privileged roles
- Business-critical data access
- Maintaining a policy’s exception list
- Asking group owners to confirm guest access
- Recurring reviews on a schedule

### Multi-Stage Access Reviews
Access reviews that occur in multiple steps or approval layers.

---

## Privileged Identity Management (PIM)
Lifecycle actions:
- Assign
- Activate
- Approve / Deny
- Extend / Renew  

PIM mitigates risks of excessive, unnecessary, or misused access by enforcing:
- Time-based role activation
- Approval-based activation

---

## Microsoft Entra ID Protection
Uses security signals to identify, manage, control, and monitor identity-based risks and threats.

---

## Microsoft Entra Permissions Management
Cloud Infrastructure Entitlement Management (CIEM) solution.

Features:
- **Cross-cloud permissions discovery**: Normalized permissions visibility across AWS, Azure, and GCP.
- **Permission Creep Index (PCI)**: Measures risk from unused or excessive permissions.
- **Permission usage analytics**: Multi-dimensional visibility into permission risks across identities, actions, and resources.

---

## Microsoft Entra Verified ID

### Issuer
An organization that verifies claims and issues digitally signed credentials.
Examples: government agencies, employers, universities.

### User
Receives, approves, stores, and presents credentials from a digital wallet.
Credentials are cryptographically signed with the user’s private key.

### Verifier
Requests proof and validates credential claims.
Examples: employers, airlines, mortgage companies.

---

## Key Concepts and Clarifications

- **Microsoft Entra Terms of Use**: Presents information to users before access and can require acceptance.
- **Microsoft Entra Identity Protection**: Uses security signals to identify potential identity threats.
- **Azure Identity Protection**: Same purpose as Entra Identity Protection.
- **Microsoft Defender**: Protects endpoints only; not for identity threat mitigation.

---

## Entitlement Management
Best for project-based access needs.
Automates:
- Access requests
- Assignments
- Reviews
- Expiration of access packages

---

## Security Tools Comparison

- **Privileged Identity Management (PIM)**: Mitigates risks from excessive privileged access.
- **Identity Protection**: Detects and responds to identity-based threats.
- **Permissions Management**: Multicloud visibility and remediation across Azure, AWS, and GCP.

---

## Microsoft Entra ID Capabilities
- Provides SSO and federation
- Acts as one perimeter in defense-in-depth
- Does NOT provide file services
- Does NOT encrypt data in transit

---

## Password and Access Security
- **Microsoft Entra Password Protection**: Helps defend against password spray attacks.
- **Conditional Access**: Enforces policies using signals but does not stop password attacks alone.
- **Self-Service Password Reset (SSPR)**: Allows users to reset passwords but does not prevent attacks.
- **Windows Hello for Business**: Replaces passwords with strong two-factor authentication.

---

## RBAC Comparison

### Microsoft Entra RBAC
Controls access to Microsoft Entra resources using built-in and custom roles.

### Azure RBAC
Controls access to Azure resources.

RBAC concept applies to both, but they manage different resource scopes.

---

## External Identity Access

- **Microsoft Entra External ID**: Allows external users to sign in using social, enterprise, or local accounts with SSO.
- **Microsoft Entra B2B**: Enables sharing apps and services with guest users.
- **Active Directory Domain Services (AD DS)**: Does NOT support social identity authentication.
- **Active Directory Web Services (ADWS)**: Provides a web service interface to AD DS and AD LDS.
