# Build Automation with Power Automate

## Common Scenarios and Capabilities
- Automating repetitive tasks such as moving data from one system to another.
- Guiding users through a defined process (for example, guiding sales teams through sales stages).
- Automating desktop-based and website processes using Robotic Process Automation (RPA).  
  Example: Automatically logging into a website, retrieving exchange rates, saving them locally, and updating a spreadsheet.

---

## Types of Flows

### Business Process Flows
- Used in model-driven apps.
- Guide users through stages and steps of a business process.
- Focused on completing processes to a defined conclusion.

### Cloud Flows
- Most commonly used flow type.
- Start with a trigger (email received, social media mention, record created).
- Perform actions such as creating records, sending emails, or requesting approvals.

### Desktop Flows
- RPA-based flows.
- Record actions performed on a desktop or in a web browser.
- Can pass data in and out of the automation.
- Useful for automating manual, UI-based processes.

---

## Cloud Flow Types
- Automated flows  
- Instant flows  
- Scheduled flows  

---

## Power Automate Interfaces
- Power Automate Portal  
- Power Automate Mobile  
- Power Automate Desktop  

---

## Components of a Cloud Flow

### Trigger
Determines what starts the flow.  
A flow has **only one trigger**.

Common trigger types:
- When something changes  
- On a schedule  
- On a button press  

### Actions
Determine what the flow does after it starts.

---

## Process Mining
Used to:
- Improve operational efficiency  
- Enhance customer experience  
- Optimize resources  
- Ensure compliance  
- Improve supply chain management processes  

### Process Mining Templates

#### Azure Templates
- Azure DevOps (work tracking)
- Azure DevOps (pipelines)
- Logic Apps (standard plan)
- Logic Apps (consumption plan)
- Durable Functions

#### Finance and Operations Templates
- Accounts payable
- Procure to pay
- Visualizations and KPIs

#### Power Platform Templates
- Desktop flows analysis
- Power Apps analysis

---

## Cloud Flows
- Primarily used to automate processes using APIs.
- Use connectors to integrate with cloud services.

### Cloud Flow with Copilot
- Uses AI assistance to help build and manage flows.

---

## Desktop Flows
- Run on a local machine.
- Created using Power Automate for Desktop.
- Can be triggered manually or by cloud flows.
- Commonly used for UI automation (websites, desktop apps).

### Desktop Flow Components
- Toolbar  
- Subflows  
- Actions Pane  
- Workspace  
- Input/Output Variables  
- Flow Variables  

### Recorder
- Records user actions on websites, desktop apps, or browsers.
- Captured steps can be edited in the designer.

---

## Flow Logic and Control

- **Action**: Performs an operation in a flow.
- **Trigger**: Starts a flow but does not perform actions like sending emails.
- **Condition**: Executes actions based on true/false logic.
- **Loop**: Iterates over items in a collection.

### Loop Types
- Apply to each: Loops through items in a collection.
- Do until: Loops until a condition is met.
- Switch: Executes different actions based on an input value.

---

## Approvals
- Microsoft Teams includes an Approvals app to view approvals and their status.
- Power Automate portal shows approvals under Action Items.
- Business process flows do **not** show approvals.
- Canvas apps can start approvals but cannot monitor their status.
- Maker portal cannot display approval action items.

---

## Error Handling and Data Actions
- **Run after**: Executes actions if a previous step fails.
- **Retry policy**: Controls retry attempts after failure.
- **Compose action**: Used to shape and transform data.

Run after, retry policy, and compose actions cannot send email notifications on failure by themselves.

---

## Flow Triggers Overview
- Automatic trigger (record updated): Used to update the triggering record.
- Automatic trigger (record created): Used to act on the newly created record.
- Instant flow: Requires manual input (button press).
- Scheduled flow: Runs at defined times and frequencies.
- Business process flows: Guide users through business steps.

---

## Connectors and APIs
- Premium HTTP connector and custom connectors can call custom APIs.
- Word Online (Business) and Excel Online (Business) connectors work only with files supported by Microsoft Graph.
- Dataverse connector works only with Dataverse data.
- Business process flows cannot interact with custom APIs.

---

## Solution Design Notes
- Automatic cloud flows can be triggered using SharePoint Online connectors.
- Connectors are required for SharePoint Online and Exchange Online.
- Power Apps are used for UI and forms (not required if no UI is needed).
- Power BI is used for data visualization (not required if no visualization is needed).
- Copilot Studio is used for chatbot-based interaction (not required if no user interaction exists).

---

## Custom Connectors
- Used when integrating with custom web applications.
- Created based on API documentation.
- Licensing, connection user, or security role does not change available connector actions.
