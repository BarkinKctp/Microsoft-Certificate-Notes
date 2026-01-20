# Build Apps with Power Apps

## Power Apps
Power Apps is a no-code/low-code platform for building apps that builds off concepts like formulas in an Excel workbook such as `SUM` and `TEXT`. You can use Power Apps to build simple solutions. If you can envision an app to solve a business problem, then you can use your existing skills to build it.

Although Power Apps can be used by virtually anyone, it also offers advanced functionality for seasoned developers to design complex applications with ease.

With Power Apps, you have choices. With hundreds of connectors, you can easily connect to data, using the underlying data service and app platform Microsoft Dataverse or a multitude of online and on-premises data sources.

### Common Data Sources
- Dataverse  
- SharePoint  
- Dynamics 365  
- SQL Server and Azure SQL  
- Office 365  

Power Apps supports multiple data connections, allowing you to bring data together from many platforms into a single app.

There are two primary application types that can be created with Power Apps:
- Canvas apps  
- Model-driven apps  

---

## Canvas Apps
Canvas apps created in Microsoft Power Apps are a great option for organizations to build tailored apps designed to perform specific tasks based on their needs. A key advantage of canvas apps is that they interact with data from multiple data sources.

Once created, canvas apps can be easily shared with users so they can run them in a browser or on a mobile device. Canvas apps can also be embedded into:
- SharePoint sites  
- Power BI reports  
- Model-driven applications  
- Microsoft Teams  

Canvas apps are easy to create and can be built from existing data such as:
- Excel spreadsheets  
- SharePoint lists  

Applications designed in Figma can also be converted into Power Apps.

If you do not need a custom design and your data is in Microsoft Dataverse, you can automatically generate a model-driven app.

---

## Model-Driven Apps
Unlike canvas apps, where the app maker controls the data sources, screen layout, and user experience, model-driven apps are always built on Microsoft Dataverse.

Model-driven apps use a data-first design approach. App design focuses on adding components such as:
- Forms  
- Views  
- Charts  
- Dashboards  

These components are added to tables using an app designer tool.

Model-driven apps are responsive by default and work across:
- Browsers  
- Mobile phones  
- Tablets  

Model-driven applications are typically used as management applications.

You define relationships, forms, views, business rules, and more at the Dataverse layer. These definitions provide enough control to meet business requirements without writing extensive formulas.

---

## Canvas vs Model-Driven Apps
Most solutions contain a combination of both canvas and model-driven apps.

---

## Power Apps Components
- Power Apps Studio  
- App Format  
- Connectors  
- Galleries  
- Forms  
- Input Controls  
- Intelligent Controls  
- Functions  
- Responsive Containers  

---

## Power Apps Controls
- **Galleries**: Layout containers that display multiple records from a data source.  
- **Forms**: Display details about data and allow record creation and editing.  
- **Media**: Include images, camera controls, barcode readers, and more.  
- **Charts**: Enable instant data analysis within the app.  

---

## Model-Driven App Components

### Data
- Table  
- Column  
- Relationship  
- Choice  

### UI
- App  
- Site map  
- Form  
- View  

### Logic
- Business process flow  
- Business rule  
- Flows  

### Visualization
- Chart  
- Dashboard  
- Embedded Microsoft Power BI  

---

## Additional Notes
- Power BI reports or dashboards can be embedded inside a Power Apps portal.  
- Microsoft Copilot Studio bots can be integrated into Power Apps portals.  
- Power Automate is used to create automated workflows between applications and services.  
- Canvas apps are not intended for external users.  

---

## Environments
- **Sandbox environment**: Used for development and testing, separate from production. Apps can be shared with any user in the associated Microsoft Entra ID tenant.  
- **Trial environment**: Limited to a single user and expires after 30 days.  
- **Dataverse for Teams environment**: Restricted to members of the associated team.  
- **Default environment**: Cannot be backed up.  

---

## Security in Model-Driven Apps
Model-driven apps use role-based security to control access to:
- The app  
- App features  
- App data  

A model-driven app is associated with one or more Dataverse security roles. Users must be assigned one of these roles to access the app. When sharing the app, you must also share the relevant security roles.

---

## Scenario: Project Request App
You build a canvas app for users to request a new project with the following requirements:
- Project information is stored in a SharePoint Online list.  
- When a new item is added, a new Microsoft Teams team is created automatically.  

### Required Actions
- Add a connection to Microsoft Teams.  
- Create an automated cloud flow.  

A Microsoft Teams connection is required to create teams. An automated cloud flow must trigger when a new item is added to the SharePoint list. An instant flow is not suitable because it requires manual triggering.

---

## UI and Controls
- The color of a label’s text can be changed using the color picker or by setting the `Color` property.  
- The `Fill` property sets the background color of a control, not the text color.  

---

## Portal Apps
A portal app using the Partner portal template allows users to:
- Self-register for access  
- Read documentation through the knowledge management feature  

Canvas apps require explicit sharing with each external user and cannot support self-service registration. Model-driven apps also do not support self-service registration.

Cloud flows do not provide a user interface and cannot be used as a web-based user-facing solution.

---

## Sitemap and Navigation
- A **subarea** can show tables, dashboards, or custom pages.  
- Multiple subareas can be added to a group.  
- A **group** cannot directly show a table.  
- An **area** can have multiple groups but cannot show tables.  
- The **command bar** displays context-specific menu items and is not part of sitemap navigation.  

---

## Scenario: Sharing a Model-Driven App
You create a model-driven app using a custom Dataverse table with no privileges assigned. To share the app with a user, you must:
- Assign a security role to the custom table.  
- Share the app with the user and assign a security role.  

Incorrect actions include setting the user as a co-owner or sharing the app link without permissions.

---

## Views and Forms
- The **view designer** controls:
  - Visible columns  
  - Row filters  
  - Sorting behavior  

- The **app designer** determines which views are included in the app.  

In model-driven apps:
- Forms allow users to view or edit records.  
- New columns added to a table must be added to forms and published to be visible.  
- Adding a column to a view does not allow editing of that column.  

---

## Model-Driven App Characteristics
- Use a single data source: Microsoft Dataverse  
- Navigation is based on Dataverse relationships  
- Predefined, responsive UI  
- Support components such as Power BI dashboards and business process flows  
- No-code components that do not require Power Fx for functionality or navigation  
