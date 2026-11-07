# DnD Trading Website — Legacy Copy

> **Earlier portfolio copy.** The [current DnD Trading Website repository](https://github.com/DarianRobert/DnD-Trading-Website) contains the original team commit history and is the version linked from my portfolio. This repository is retained as an older snapshot.

An ASP.NET Web Forms application developed for a stationery distribution business as part of a University of KwaZulu-Natal team project in 2025.

The website includes customer-facing product and order pages alongside client and supplier management screens. It complements the [DnD Trading desktop application](https://github.com/DarianRobert/DnD-Trading).

## Technology

| Component | Technology |
| --- | --- |
| Web framework | ASP.NET Web Forms with C# code-behind |
| Runtime target | .NET Framework 4.7.2 |
| Database and access | SQL Server, ADO.NET (`SqlConnection`, `SqlCommand`, `SqlDataAdapter`) |
| Frontend | HTML, CSS, JavaScript, Bootstrap, jQuery |
| Local development | Visual Studio, IIS Express, NuGet |

## Features represented in the source

- Product browsing and checkout pages.
- Login, client details, and client order pages.
- Supplier and supplier product pages.
- Order and report pages.
- Contact and order email functionality.

## My contribution

I led the wider DnD Trading project team, coordinated development goals and timelines, and contributed to frontend and backend development across the project. This repository contains the team's website component.

## Repository layout

The original solution is currently stored in `DNDWebsite (2).zip`. After extraction, the web project and solution are inside `DNDWebsite/DNDWebsite/`.

| Path inside the web project | Purpose |
| --- | --- |
| `DNDWebsite.sln`, `DNDWebsite.csproj` | Visual Studio solution and web application project |
| `Default.aspx`, `Products.aspx` | Landing and product pages |
| `Login.aspx`, `Clients.aspx`, `EditClient.aspx` | Login and client pages |
| `Checkout.aspx`, `Order.aspx`, `ClientOrders.aspx` | Checkout and order pages |
| `Supplier.aspx`, `SupplierProducts.aspx` | Supplier pages |
| `Report.aspx`, `Contact.aspx` | Reports and contact pages |
| `Site.Master` and `.aspx.cs` files | Shared layout and C# page logic |
| `Web.config` | Web application and database configuration |
| `packages.config` | NuGet dependency versions |

## Development setup

1. Install Visual Studio with the **ASP.NET and web development** workload and the **.NET Framework 4.7.2 targeting pack** on Windows.
2. Extract the archive and open `DNDWebsite/DNDWebsite/DNDWebsite.sln`.
3. Restore the packages listed in `packages.config` using Visual Studio's NuGet package restore.
4. Prepare an isolated SQL Server development database and configure `DNDConnectionString` in your local `Web.config` for it. The page code expects the original application's database tables and relationships.
5. Configure a test email service before exercising contact or order email actions.
6. Select IIS Express and start the application from Visual Studio.

## Current limitations

- Source is supplied as an archive, so GitHub cannot display the individual pages and C# files directly.
- A database provisioning script and sample dataset have not yet been packaged.
- Email workflows need environment-specific configuration.
- A clean Windows/IIS Express run and the application workflows have not yet been verified on a fresh development environment.

## Related work

- [DnD Trading desktop application](https://github.com/DarianRobert/DnD-Trading)
- [My project portfolio](https://darianrobert.github.io/)

