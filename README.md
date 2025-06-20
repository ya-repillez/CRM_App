# CRM_App - Carnet d’adresses enrichi

## Description
Application web (Blazor Server) avec backend ASP.NET Core pour gestion de contacts, interactions, et tags, synchronisation Outlook (Microsoft Graph API).

## Technologies
- Backend : ASP.NET Core 7, Entity Framework Core
- Frontend : Blazor Server
- Base de données : SQL Server
- Authentification : JWT + rôles
- Synchronisation : Microsoft Graph API (OAuth2)
- Stockage documents : Google Drive (via API)

## Installation locale

1. Cloner ce repository  
```bash
git clone https://github.com/ya-repillez/CRM_App.git


CRM_App/
├── README.md
├── CarnetContacts.sln
├── /CarnetContacts.API/
│   ├── CarnetContacts.API.csproj
│   ├── Program.cs
│   ├── appsettings.json
│   ├── Controllers/
│   │   ├── ContactsController.cs
│   │   ├── InteractionsController.cs
│   │   ├── TagsController.cs
│   │   └── AuthController.cs
│   ├── Data/
│   │   ├── ApplicationDbContext.cs
│   │   ├── Entities/
│   │   │   ├── Contact.cs
│   │   │   ├── Interaction.cs
│   │   │   ├── Tag.cs
│   │   │   └── User.cs
│   │   └── Migrations/
│   └── Services/
│       ├── OutlookService.cs
│       └── AuthService.cs
├── /CarnetContacts.Web/
│   ├── CarnetContacts.Web.csproj
│   ├── Program.cs
│   ├── Pages/
│   │   ├── Index.razor
│   │   ├── Contacts.razor
│   │   ├── Interactions.razor
│   │   ├── Tags.razor
│   │   └── Login.razor
│   ├── Shared/
│   │   ├── MainLayout.razor
│   │   └── NavMenu.razor
│   └── wwwroot/
│       └── css/
│           └── site.css
├── /SQL/
│   ├── CreateDatabase.sql
│   ├── Tables.sql
│   └── SeedData.sql
└── /Docs/
    ├── DatabaseSchema.png
    └── ArchitectureDiagram.png
