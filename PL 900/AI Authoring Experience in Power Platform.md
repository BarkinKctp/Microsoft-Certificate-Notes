# AI Authoring Experience in Power Platform

## Copilot Studio
Copilot Studio enables organizations to:
- Get started in seconds  
- Empower subject matter experts  
- Enable rich, natural conversations  
- Enable copilots to take actions  
- Extend existing copilots  
- Monitor and improve copilot performance  

---

## Components of Copilot Studio
- Topics  
- Entities  
- Actions  
- Generative AI  
- Publishing  

---

## Creating a Basic Copilot
Steps:
- Create a copilot  
- Build topics for the copilot  
- Add generative AI as needed  
- Test the copilot  
- Publish and deploy to selected channels  

---

## AI Builder
AI Builder is a Microsoft Power Platform capability that provides AI models to optimize business processes.

### AI Hub
A centralized area that provides access to:
- Prompts  
- AI Models  
- Document Automation  

---

## AI Builder Model Types
- **Prebuilt models**: Add intelligence without collecting or training data.
- **Custom models**: Built and trained from scratch for targeted solutions.

### Prebuilt AI Models
- Business card reader  
- Category classification  
- Entity extraction  
- ID reader  
- Invoice processing  
- Key phrase extraction  
- Language detection  
- Receipt processing  
- Sentiment analysis  
- Text recognition  
- Text translation  

---

## Copilot Studio Concepts

### Actions
- Used to call Power Automate cloud flows
- Can retrieve data from Microsoft Dataverse tables

### Topics
- Control the flow of conversations
- Represent categories of user intent
- Use trigger phrases to route conversations

### Entities
- Map natural language to real-world concepts
- Examples: phone number, zip code, city, person name

#### Entity Types
- **Prebuilt entities**: Phone number, zip code, email, age, etc.
- **Custom entities**: Domain-specific values (optional if prebuilt entities exist)

### Channels
- Define where a copilot is available (for example, Microsoft Teams)

### Variables
- Store user responses for later use in conversations

---

## AI Builder and Power Automate
- After training and publishing, AI Builder models become available in Power Automate cloud flows
- Renaming a model does not affect availability
- Adding training data does not affect availability
- Environment Maker role is sufficient to use AI Builder models in flows
- Basic User role is insufficient

---

## Connectors and Integrations
- Custom connectors connect to custom APIs
- AI Builder connector adds intelligence to flows
- Dataverse connector performs data operations on Dataverse only
- Dataverse connector cannot fetch data from custom portals

---

## Copilot Deployment Differences

### Copilot Studio in Microsoft Teams
- Accessible only to internal users
- Deployable only to Microsoft Teams
- Requires Microsoft 365 subscription
- Templates are available

### Copilot Studio Web App
- Can be accessed by external users
- Can be embedded in websites
- Requires additional licenses to edit copilots
- Templates are not available

---

## Conversation Design Elements
- **Trigger phrases**: Teach the copilot how users ask for topics
- **Ask a question node**: Collects user input
- **Call an action node**: Calls Power Automate flows or authentication
- **Show a message node**: Displays responses to users

These nodes do not train the copilot to recognize user phrases.

---

## Power Automate Integration
- Copilots can call Power Automate cloud flows
- Cloud flows can connect to Dataverse
- Connectors cannot be added directly to copilots
- Topics define conversations
- Entities assist with natural language understanding

---

## AI Builder Model Lifecycle
- Create  
- Train  
- Publish  
- Test  

Publishing a model makes it available only to the maker unless explicitly shared. Training or publishing alone does not grant user access.
