# Azure App Services & Related Azure Services for ASP.NET Core

## Azure App Services

  -----------------------------------------------------------------------
  Azure Service           Purpose                 Best For
  ----------------------- ----------------------- -----------------------
  Azure App Service (Web  Host ASP.NET Core web   Websites, REST APIs
  Apps)                   apps and APIs           

  Azure App Service       Isolated, private App   Enterprise applications
  Environment (ASE)       Service                 

  Azure Functions         Serverless event-driven Background jobs, APIs,
                          code                    automation

  Azure Static Web Apps   Host static frontends   React, Angular, Vue,
                          with API integration    Blazor WASM

  Azure Container Apps    Run containerized apps  Microservices, APIs
                          without Kubernetes      

  Azure Kubernetes        Managed Kubernetes      Large-scale
  Service (AKS)           clusters                containerized apps

  Azure Container         Run single containers   Batch jobs, testing
  Instances (ACI)         on demand               

  Azure Spring Apps       Managed Spring Boot     Java applications
                          hosting                 
  -----------------------------------------------------------------------

## Common Supporting Azure Services

### Database

-   Azure SQL Database
-   Azure SQL Managed Instance
-   Azure Database for PostgreSQL
-   Azure Database for MySQL
-   Azure Cosmos DB
-   Azure Cache for Redis

### Storage

-   Azure Blob Storage
-   Azure Files
-   Azure Queue Storage
-   Azure Table Storage
-   Azure Data Lake Storage Gen2

### Identity & Security

-   Microsoft Entra ID (Azure AD)
-   Azure Key Vault
-   Azure Managed Identity
-   Azure Application Gateway
-   Azure Front Door
-   Azure Web Application Firewall (WAF)

### Monitoring

-   Azure Monitor
-   Application Insights
-   Log Analytics Workspace
-   Azure Alerts
-   Azure Dashboard

### Networking

-   Azure Virtual Network (VNet)
-   Private Endpoint
-   Network Security Groups (NSG)
-   Azure Load Balancer
-   Azure DNS

### DevOps & CI/CD

-   Azure DevOps
-   GitHub Actions
-   Azure Container Registry (ACR)
-   Azure Artifacts
-   Azure Pipelines

### Messaging

-   Azure Service Bus
-   Azure Event Grid
-   Azure Event Hubs
-   Azure Notification Hubs

### API Management

-   Azure API Management (APIM)
-   Azure API Center

### AI & Search

-   Azure AI Foundry
-   Azure AI Search
-   Azure OpenAI Service
-   Azure AI Document Intelligence
-   Azure AI Vision

### Integration

-   Azure Logic Apps
-   Azure Automation
-   Azure Data Factory

### Backup & Disaster Recovery

-   Azure Backup
-   Azure Site Recovery

## Typical ASP.NET Core Production Architecture

``` text
Users
   │
Azure Front Door
   │
Application Gateway (WAF)
   │
Azure App Service
   │
Azure API Management
   │
ASP.NET Core Web API
   │
 ├── Azure SQL Database
 ├── Azure Cache for Redis
 ├── Azure Blob Storage
 ├── Azure Service Bus
 ├── Azure Key Vault
 └── Application Insights
```
