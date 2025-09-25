# OmnicoreMeetingMinutes

ASP.NET Core MVC web app for capturing and managing team meeting minutes.  
Built for Omnicore Technologies to simplify note-taking and action tracking.

![Cover](../docs/screenshots/OmnicoreMeetingMinutes-cover.png)

## ✨ Features
- Create & edit meeting minutes
- Assign action items with owners and deadlines
- Track status of tasks (open, in progress, done)
- Search and filter minutes
- Clean Bootstrap-styled UI

## 🧱 Tech Stack
- ASP.NET Core MVC (.NET 8), C#
- Entity Framework Core + SQL Server
- Bootstrap 5 for UI

## 🚀 Quick Start
### Prerequisites
- .NET 8 SDK
- SQL Server (LocalDB or full)
- Update `appsettings.json` with your connection string

### Run
```bash
dotnet restore
dotnet ef database update
dotnet run
