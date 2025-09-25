
# AgriEnergyConnect

Role-based ASP.NET Core MVC app for managing farmers, products, and employees.

![Cover](../docs/screenshots/AgriEnergyConnect-cover.png)

## ✨ Features
- Login + role-based access (employee/admin)
- CRUD for Farmers & Products
- Product filtering by category/date
- Server-side validation + Bootstrap UI
- Session-based login tracking (username/role ribbon)
- Flash messages for login/register/logout

## 🧱 Tech Stack
- ASP.NET Core MVC (.NET 8), C#
- Entity Framework Core + SQL Server
- Bootstrap 5, Razor Views

## 🚀 Quick Start
### Prerequisites
- .NET 8 SDK  
- SQL Server LocalDB or SQL Server
- Update your **appsettings.json** with a local connection string

### Run (dev)
```bash
dotnet restore
dotnet ef database update    # if migrations included
dotnet run
