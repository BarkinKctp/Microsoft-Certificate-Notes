# Identify Foundational Components of MS Power Platform

## POWER PLATFORM ADMINISTRATION

### Power Platform Environments
- Each environment is created under a Microsoft Azure Active Directory (Azure AD) tenant.
- Only users within that tenant can access its resources.
- An environment is bound to a geographic location.
- All items created in an environment (connections, gateways, Power Automate flows, etc.) are bound to that environment’s location.

---

## Power Platform Admin Center
Settings are grouped into categories accessible from the left-hand navigation:

- **Home** – Overall information and service disruptions
- **Environments** – Lists all environments (Dataverse, Dataverse for Teams)
- **Analytics** – Dataverse analytics, Flow statistics, Power Apps details
- **Billing** – User license information
- **Settings** – Tenant-level controls
- **Resources** – Capacity statistics and Dynamics 365 features
- **Help + Support** – Create and manage support requests
- **Data Integration** – Monitor Dataverse integrations (SQL, Salesforce)
- **Data** – Manage data sources and gateways
- **Policies** – Data security policies, Customer Lockbox, tenant isolation
- **Admin Centers** – Access Microsoft 365, Azure AD, and other admin portals

---

## Power Apps Maker Portal
- **Tables** – Manage Dataverse tables, forms, views, relationships
- **Connections** – Manage app connections
- **Flows** – View and manage flows
- **Chatbots** – Manage bots
- **AI Models** – Access AI Builder models
- **Solutions** – Manage deployed solutions
- **Cards** – Manage cards
- **Choices** – Manage choice columns
- **Dataflows** – Manage dataflows
- **Power Platform** – Access other maker portals

---

## Managed Environments
- Limit sharing
- Weekly usage insights
- Data policies
- Pipelines in Power Platform
- Solution checker

---

## Security and Governance
- Power Platform follows the Security Development Lifecycle (SDL).
- **Data Loss Prevention (DLP) Policies**
  - Prevent unintentional data exposure
  - Defined at environment or tenant level
  - Connector classifications:
    - **Business** – Business-use data
    - **Non-Business** – Personal-use data
    - **Blocked** – Restricted connectors
  - All connectors default to Non-Business when a policy is created
- Compliance and data privacy
- Data protection
- Accessibility

---

## Microsoft Dataverse
Microsoft Dataverse is a cloud-based data platform for structured data and business logic.

- **Security** – Azure AD auth, MFA, row/column security, auditing
- **Logic** – Business rules, workflows, duplicate detection
- **Data** – Data modeling, validation, reporting
- **Storage** – Azure-hosted, fully managed
- **Integration** – APIs, webhooks, eventing, exports

---

## Dataflows
Self-service, cloud-based data preparation using Power Query.

- Ingest, transform, and load data into Dataverse, Power BI, or Azure Data Lake
- Run on-demand or on a schedule
- Decouples transformation from visualization
- Centralized transformation logic
- Product agnostic
- Runs entirely in the cloud
- Requires no IT or developer background

---

## Common Data Model
- Standardized data structure across applications
- Enables cross-app integration
- Extensive metadata system
- Organizations can create and share custom data types

---

## Connectors
- Bridge between data sources and apps/flows
- Enable cross-platform integration
- Extend functionality across platforms

---

## Data Sources
- **Tabular data sources**
  - Structured tables
  - Support read/write operations
  - Examples: Dataverse, SharePoint, SQL Server
- **Function-based data sources**
  - Use functions for actions
  - Examples: Office 365 Users, Project Online, Azure Blob Storage

---

## Triggers
- Used only in Power Automate
- Start a flow
- Time-based or action-based
- Required for every workflow

---

## Actions
- Used in Power Automate and Power Apps
- Perform operations on data sources
- Examples: send email, create a row

---

## Connector Types
- Standard Connectors
- Premium Connectors
- Custom Connectors

==============================================================================

## Canvas App Data Handling
- Collections store temporary data and are cleared when the app closes
- `Clear()` removes collection data
- Session-specific data should not be stored in Dataverse or SharePoint
- Variables store a single value or object (not multiple items)

---

## Controls
- Combo box, dropdown, list box – select multiple values
- Radio control – mutually exclusive options
- Rating control – single value

---

## App Types and Use Cases
- **Power Pages** – External-facing users
- **Canvas & Model-driven apps** – Internal users
- **Power BI dashboards** – Data consumption (not transactional)

---

## AI and Automation
- AI Builder document processing extracts data from documents
- AI Builder models can be triggered via Power Automate flows
- Canvas apps enable screen and form interaction
- Copilot Studio enables bot interaction
- Power BI provides reports and dashboards
## Dataverse Tables
- Standard (out-of-the-box) tables included
- **Currency table** – Not an activity table
- **Activity table** – Calendar-based records
- **Custom tables** – Created directly in Dataverse
- **Virtual tables** – External data sources
