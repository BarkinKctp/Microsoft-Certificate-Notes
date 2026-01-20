# Introduction to Microsoft Power Platform

---

## Explore Microsoft Power Platform
- **Power Apps**
- **Power Automate**
- **Power BI**
- **Power Pages**

---

## Supporting Tools
- **Microsoft Copilot Studio**
- **Connectors**
- **AI Builder**
- **Dataverse**
- **Power Fx**
- **Managed Environments**

---

## Connectors
With Power Platform, data connectors make working with different data sources easier.  
They act as a bridge between data sources and your app or workflow.  
Power Platform has more than **900 connectors** available to various data sources.

---

## Microsoft Dataverse
Microsoft Dataverse allows organizations to securely store and manage data used by business applications.  
Dataverse data is stored in **tables**.

### Key Features
- **Easy to manage**: Metadata and data are stored in the cloud.
- **Easy to secure**: Role-based security ensures users access only what they need.
- **Rich metadata**: Data types and relationships are used directly within Power Apps.
- **Logic and validation**: Calculated columns, business rules, workflows, and business process flows.
- **Productivity tools**: Tables are available within Microsoft Excel add-ins.

---

## Copilot in Power Platform

### Simplify App Creation
Copilot enables fast application creation using natural language.  
You describe the app you want, and AI designs it for you.

- Generates a **Dataverse table**
- Builds a **canvas app**
- Provides in-app guidance

### Copilot in Power Apps
Users can ask questions about their data (for example, total properties in real estate apps).

### Copilot in Power Automate (Cloud Flows Designer)
- Creates a flow from a scenario prompt
- Sets up required connections
- Applies parameters automatically
- Updates or replaces actions
- Answers questions about flows

---

## Power Fx
Power Fx is the low-code language used throughout Microsoft Power Platform.

**Characteristics**
- General-purpose
- Strongly typed
- Declarative and functional
- Human-readable syntax

Designed for end users to easily learn and use.

---

## Microsoft Teams and Power Platform
Microsoft Teams is highly extensible, allowing organizations to build custom apps.  
Power Platform enables rapid development of Teams-compatible apps using low-code tools.  
All Power Platform components integrate with Microsoft Teams.

---

## Power Platform and Dynamics 365
- All Dynamics 365 customer engagement apps are **model-driven apps**
- Built on **Microsoft Dataverse**
- Created using **Power Apps**
- Use forms, views, charts, and dashboards to present data

---

## Power Platform and Azure Services
Power Platform and Azure services complement each other to:
- Modernize legacy systems
- Automate processes
- Build advanced analytics solutions

---

## AI Builder
Microsoft Power Platform includes prebuilt AI Builder models, such as:
- **Sentiment analysis** for text data
- **Entity extraction** (city, phone number, location, etc.)

AI Builder can be used in:
- Power Apps
- Power Automate flows

---

## Power BI
- Business analytics and intelligence platform
- Creates dashboards, reports, charts, and graphs
- Visualizes data from multiple sources

---

## Core Power Platform Components
- **Dataverse**: Data storage and management
- **Power Pages**: External-facing websites
- **Power Apps**: Low-code apps (canvas, model-driven, Power Pages)
- **Power Automate**: Automated workflows and approvals
- **Copilot Studio**: Natural language bots

---

## Microsoft Dataverse vs Dataverse for Teams

### Dataverse for Teams Limitations
- No auditing
- Single business unit
- No multiple currencies
- No mobile offline support

### Shared Capabilities
- File and image data types
- Power Automate integration
- Relational storage support

---

## Dataverse Column Types

### Common Column Types
- **Choice**: Single value selection (nullable)
- **Choices**: Multiple value selection
- **Yes/No**: Two values only (e.g., Approve/Reject)
- **Autonumber**: Auto-generated unique text values
- **Text**: Free user input without validation

---

## Dataverse Relationships and Keys
- One-to-many relationships create **lookup (foreign key) columns**
- **Alternate keys** support external integrations
- **Customer column** represents an account or contact
- Every table has a **primary key**

---

## Data Security and Governance

### Data Loss Prevention (DLP)
- Prevents combining business and non-business connectors
- Prevents accidental data leakage

### Other Governance Tools
- **Microsoft Entra ID Conditional Access**: Controls access, not data leakage
- **CoE Toolkit**: Monitors apps, flows, connectors
- **Auditing**: Tracks data changes, does not prevent leakage

---

## Environments
- Each environment has **one Dataverse instance**
- Required to host Dataverse

---

## Administration Portals
- **admin.powerplatform.microsoft.com**: Admin center
- **make.powerapps.com**: Build apps and manage environments
- **make.powerautomate.com**: Build flows
- **app.powerbi.com**: Create and view Power BI dashboards

---

## Advanced Security Features
- **DLP Policies**: Separate business and non-business data
- **Tenant Isolation**: Controls tenant data movement
- **Customer-managed keys**: Encrypt Dataverse environments
- **Customer Lockbox**: Approve Microsoft support access

---

## Application Types
- **Model-driven apps**: Backend, Dataverse-based, guided processes
- **Canvas apps**: Scenario-focused applications
- **Desktop flows**: Robotic Process Automation (RPA)
- **Power Pages**: External access to Dataverse data

---

## Summary
- **Power Apps**: Build low-code business apps
- **Power Automate**: Create workflows and automations
- **Copilot Studio**: Build conversational bots
- **Power BI**: Business analytics and visualization
