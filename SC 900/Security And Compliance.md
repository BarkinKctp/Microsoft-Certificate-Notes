# Security and Compliance

## Defense in Depth
Defense in depth uses a layered security approach to protect systems and data.

- **Physical security**: Restricting access to datacenters to authorized personnel only.
- **Identity and access security**: Controls such as multifactor authentication (MFA) and conditional access.
- **Perimeter security**: Distributed Denial of Service (DDoS) protection to stop large-scale attacks.
- **Network security**: Network segmentation and access controls to limit communication between resources.
- **Compute layer security**: Securing virtual machines by closing unnecessary ports.
- **Application layer security**: Ensuring applications are secure and free from vulnerabilities.
- **Data layer security**: Managing access to data and using encryption to protect business and customer data.

### CIA Triad
- **Confidentiality**
- **Integrity**
- **Availability**

### Shadow IT
Use of unauthorized applications or services outside official IT governance.

---

## Zero Trust
Zero Trust assumes that all networks are untrusted.

Principles:
- Verify explicitly  
- Least privileged access  
- Assume breach  

---

## Encryption
- **Symmetric encryption**: Uses the same key to encrypt and decrypt data.
- **Asymmetric encryption**: Uses a public and private key pair.

---

## Hashing
Converts text into a unique fixed-length value. Hashing is one-way and cannot be reversed.

---

## Governance, Risk, and Compliance (GRC)

### Data Residency
Regulations governing where data can be stored and how it can be transferred, processed, or accessed across regions.

### Data Sovereignty
Data is subject to the laws and regulations of the country or region where it is collected, stored, or processed.

### Data Privacy
Controls and policies that protect personal and sensitive data.

---

## Identity and Access

### Single Sign-On (SSO)
- Allows users to sign in once and access multiple applications.
- Uses a centralized identity provider.
- Does not guarantee users will never need to sign in again.
- Not related to password resets.

### Conditional Access
- Enforces access controls such as MFA based on conditions.
- Improves organizational security.

Conditional Access signals include:
- User or group membership  
- Named locations  
- Applications  
- Real-time sign-in risk  
- Cloud apps or actions  
- User risk  

### Password Hash Synchronization
Enables synchronization of passwords with Active Directory.

---

## Shared Responsibility Model
Defines which security responsibilities belong to the customer and which belong to the service provider.

---

## Compliance
- **PCI** is a compliance regulation, not a security model.

---

## DDoS Attacks
Common types:
- Resource layer attacks  
- Protocol attacks  
- Volumetric attacks  

Password spray and man-in-the-middle (MITM) attacks are **not** DDoS attacks.

---

## Risk Detection

### User Risk
Evaluates the likelihood that a user account has been compromised.
- Example: leaked credentials

### Sign-In Risk
Detects risky sign-in attempts.
- Examples: atypical travel, anonymous IP address, password spray

### Device State
Verifies device platform and compliance.

### Location
Associated with specific IP networks.

---

## Microsoft Security Principles
- **Security principle**: Encryption and key management.
- **Control principle**: Customers control their data.
- **Strong legal protection**: Legal access requests go to the customer, not Microsoft.
- **Transparency principle**: Clear communication on how data is used and accessed.
