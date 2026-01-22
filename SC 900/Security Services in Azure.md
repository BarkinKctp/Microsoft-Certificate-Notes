# Security Services in Azure

### Azure DDoS Protection

#### DDoS Attack Types
- **Volumetric attacks**: Flood the network with large amounts of traffic, exhausting bandwidth so legitimate traffic can’t get through.
- **Protocol attacks**: Exploit weaknesses in Layer 3 (network) and Layer 4 (transport) protocols to exhaust server resources.
- **Resource (application) layer attacks**: Target web application packets to disrupt data transmission between hosts.

#### Azure DDoS Protection Capabilities
- Always-on traffic monitoring
- Adaptive real-time tuning
- DDoS protection telemetry, monitoring, and alerting

#### DDoS Protection Options
- **DDoS Network Protection**
- **DDoS IP Protection**

---

## Azure Firewall
- Built-in high availability and availability zones
- Network and application-level filtering
- Outbound SNAT and inbound DNAT for internet communication
- Support for multiple public IP addresses
- Threat intelligence
- Integration with Azure Monitor

---

## Web Application Firewall (WAF)
- Provides application-layer protection only
- Does NOT provide network-layer filtering

---

## Network Segmentation
- **Azure Virtual Network (VNet)** is the core component for network segmentation.

---

## Azure Network Security Groups (NSG)
- Provide distributed network-layer traffic filtering
- Control inbound and outbound traffic to resources within virtual networks
- Applied at subnet or network interface level

---

## Azure Bastion
- Provides secure RDP and SSH access to virtual machines
- Access through a browser using the Azure portal
- Fully platform-managed PaaS service
- No need to expose public IPs on virtual machines

---

## Azure Key Vault
- Centralized cloud service for storing application secrets
- Stores keys, secrets, and certificates securely

---

## Key Security Concepts

- Firewalls control access between networks.
- Bastion hosts provide secure RDP and SSH access via the Azure portal.
- Security groups simplify assigning access by grouping users.
- Azure WAF provides centralized protection for web applications against common exploits and vulnerabilities.

---

## Security Standards and Benchmarks
- **Center for Internet Security (CIS)**: Primary industry security benchmark
- **National Institute of Standards and Technology (NIST)**: Used in Azure Secure Benchmark
- **Federal Information Processing Standard (FIPS) 140**: Standard for hardware security modules
- **Open Web Application Security Project (OWASP)**: WAF-related security standard
