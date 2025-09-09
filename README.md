# Inventory Aspire Sample

A sample **.NET Aspire** solution demonstrating:

- **Distributed application orchestration** with .NET Aspire
- **Service discovery** between projects (no hard‑coded URLs)
- **Blazor WebAssembly** frontend
- **Blazor Server** frontend
- **ASP.NET Core Web API** backend
- Shared DTOs and clean API consumption patterns

---
## 🚀 Features

- **.NET Aspire Orchestration**  
  All projects are registered in the AppHost with `WithReference` and `WaitFor` to ensure correct startup order.

- **Service Discovery**  
  Blazor Server resolves API endpoints dynamically via `https+http://api` — no hard‑coded ports.

- **Multiple Frontends**  
  - Blazor WebAssembly (direct API calls with configured base URL)
  - Blazor Server (API calls via service discovery)

- **Shared Contracts**  
  DTOs can be placed in a shared project to avoid duplication.

---

## 🛠 Prerequisites

- [.NET 9 SDK](https://dotnet.microsoft.com/download)
- Visual Studio 2022 (17.10+) or VS Code with C# Dev Kit
- SQL Server LocalDB or another SQL provider (if your API uses a database)

---
