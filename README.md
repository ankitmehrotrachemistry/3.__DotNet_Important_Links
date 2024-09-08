# DotNet_Important_Links

#### 1). CORS (Cross Origin Resource Sharing)

- Cross-Origin Resource Sharing (CORS) is a security feature that allows or restricts web applications running at one domain to make requests for resources from a different domain.  
- In a .NET Core API, CORS is implemented using middleware.   
- A CORS policy defines which domains, HTTP methods, headers, and other options are permitted. 
- You need to register the CORS middleware in the Configure method of Startup.cs .
  
'app.UseCors("AllowSpecificOrigin");'

 [Cross-Origin Resource Sharing in .NET](https://medium.com/@darshana-edirisinghe/cross-origin-resource-sharing-in-net-f8d0aa802b5f)

#### 2). How to handle Exception except try-Catch?

- 

#### 3). Routing in WEB API and MVC

- 

#### 4). Middleware and it's working

- 

#### 5). Create Custom Middleware

- 

#### 6). OWIN Middleware

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)

#### 7). Dependency Injection

- [ASP.NET Core Dependency Injection](https://www.ezzylearning.net/tutorial/a-step-by-step-guide-to-asp-net-core-dependency-injection)

#### 8). AddScoped, AddTransient and AddSingleton

- [Dependency Injection and using AddTransient, AddScoped and AddSingleton in an ASP.NET Core application](https://alexb72.medium.com/dependency-injection-and-using-addtransient-addscoped-and-addsingleton-in-an-asp-net-2ae09e45c983)

- [Navigating Dependency Lifetimes: A Practical Comparison of AddTransient, AddScoped, and AddSingleton in .NET](https://nshyamprasad.medium.com/navigating-dependency-lifetimes-a-practical-comparison-of-addtransient-addscoped-and-8b825a465dc5)

#### 9). Extension Methods - App.Run() and App.Use()

Extension methods are a way to add new functionality to existing types without modifying their source code. They are static methods that can be called as if they are instance methods on the extended type.

In one of my .NET Core projects, I created an extension method for validating email addresses. 

```csharp
public static class StringExtensions
{
    public static bool IsValidEmail(this string email)
    {
        return Regex.IsMatch(email, @"^[^@\s]+@[^@\s]+\.[^@\s]+$");
    }
}


app.UseRouting(): This is used to route incoming requests to the appropriate handlers (e.g., player connections, game events).
app.UseWebSockets(): If you are handling real-time communication, WebSockets may be necessary for live multiplayer game servers.
app.UseEndpoints(): Configures endpoints for different routes like /api/game/start for starting a game or /api/game/player/connect for player connections.

- 

#### 10.1). Entity Framework Core

- [Entity Framework Core Model](https://www.learnentityframeworkcore5.com/entity-framework-core-model)
  
- [One-to-Many Relationships using Fluent API in Entity Framework Core](https://www.entityframeworktutorial.net/efcore/configure-one-to-many-relationship-using-fluent-api-in-ef-core.aspx)

- [An Insightful Dive into Entity Framework Core](https://www.linkedin.com/pulse/insightful-dive-entity-framework-core-heart-data-management-adi-inbar/?trackingId=CKg92x8pLiei6Du9gH2AjQ%3D%3D)

- ▶️ [Complete 3 Hour ASP NET 6.0 and Entity Framework Core Course!](https://www.youtube.com/watch?v=7d2UMAIgOLQ&list=PLwhVruPHD9rxZ9U5K6vqUFkfrjaRhwEsV&index=12)

#### 10.2). DataBase First Approach and CodeFirst Approach

🎮 Store persistent player data (e.g., profiles, achievements, leaderboards) using a database like SQL Server. Use Entity Framework Core (Code First) to interact with the database.

- [Entity Framework Core Model](https://www.learnentityframeworkcore5.com/entity-framework-core-model)
 
#### 10.3). DbContext

- [DbContext](https://www.learnentityframeworkcore5.com/dbcontext)

- [c# Entity framework core assignment solution: Add models and tables](https://www.linkedin.com/pulse/c-entity-framework-core-assignment-solution-add-models-adi-inbar-3r87f/?trackingId=dxMHMLu80K4bLf%2B8FpVmzA%3D%3D)

- [ASP.NET Core REST API DbContext](https://www.pragimtech.com/blog/blazor/asp.net-core-rest-api-dbcontext/)
 
#### 10.4). LINQ

- [Mastering C# LINQ Guide](https://www.bytehide.com/blog/linq-csharp)

- [LINQ Interview Questions and Answers](https://vasistadotnet.wordpress.com/wp-content/uploads/2015/02/linq-interview-questions-answers-by-shailendra-chauhan.pdf)

- [Top 100 LINQ Interview Questions](https://github.com/Devinterview-io/linq-interview-questions) 
 
#### 10.5). Migrations

- [Migrations in Entity Framework Core](https://www.entityframeworktutorial.net/efcore/entity-framework-core-migration.aspx)

- [Navigating Migrations and Delete Table in Entity Framework Core](https://www.linkedin.com/pulse/navigating-migrations-delete-table-entity-framework-core-adi-inbar/)

- [Harnessing Entity Framework Core: Add Migration in C#](https://www.linkedin.com/pulse/harnessing-entity-framework-core-add-migration-c-adi-inbar/?trackingId=VnxXh8XGAjpfVSfRaFG39A%3D%3D)

- [Reverting and Managing Migrations in Entity Framework Core with C#](https://www.linkedin.com/pulse/reverting-managing-migrations-entity-framework-core-c-adi-inbar/?trackingId=w3J1ieu5fLpAMDfIVaruhA%3D%3D)
 
#### 10.6). Seeding Data

- [Migration Seeding Data in Entity Framework Core with C#](https://www.linkedin.com/pulse/seeding-data-entity-framework-core-c-adi-inbar-tqwff/?trackingId=Bgt89Mt6yxrDPsRHDmpSOQ%3D%3D)

- [EF Core Seed Data](https://www.learnentityframeworkcore.com/migrations/seeding)
 
#### 10.7). Nullable

- [Understanding Nullable Fields and Renaming Columns in C# with Entity Framework Core](https://www.linkedin.com/pulse/understanding-nullable-fields-renaming-columns-c-entity-adi-inbar/?trackingId=%2BwnxToGDylnTUiTV54QnEA%3D%3D)
 
#### 10.8). Entity States

- [Entity States in Entity Framework](https://dotnettutorials.net/lesson/entity-state-in-entity-framework/)

#### 11). JWT Authentication and Role Based Authorization

🎮 Use JWT Tokens for player authentication, especially in multiplayer environments where players need to remain authenticated across multiple sessions.

- [OAuth 2.0 and OpenID in simple terms](https://medium.com/@iamprovidence/oauth-2-0-and-openid-in-simple-terms-7196089a1b29)

#### 12). Kestrel Server

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)

#### 13). State Management - Client and Server

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)

#### 14). Session Management

Sessions in Web Applications refer to the mechanism of storing user-specific data temporarily on the server side across multiple requests. Unlike cookies, which are stored on the client side, session data is stored on the server side, enhancing security and reducing the risk of exposing sensitive information.
Sessions typically generate a unique identifier (session ID) for each user session upon their first interaction with the application. This identifier (session ID) is stored as a cookie on the client side (usually), and the corresponding data is stored on the Web Server. When the client makes subsequent requests, this session ID is sent in the Request header. The server uses this identifier to retrieve session-specific data stored in memory (Temporary Caching Mechanism), a database, or another persistent storage mechanism. This data persists until the session expires (due to user inactivity or logout) or is manually cleared.

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)

#### 15). .NET Core and .NET Middleware

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)

#### 16). Filters and it's type

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)

#### 17). What is MVC Architecture? How to create Controllers?

- 

#### 18). Controller Action Methods in MVC

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)

#### 19). What are Views? ViewData , ViewBag and TempData

- [ASP.NET MVC: Models, ViewData, ViewBag, and TempData Explained](https://www.linkedin.com/pulse/aspnet-mvc-models-viewdata-viewbag-tempdata-explained-ervis-trupja-ytn7f/)

#### 20). Repository Pattern

- [Repository Pattern Implementation in ASP.NET Core](https://medium.com/net-core/repository-pattern-implementation-in-asp-net-core-21e01c6664d7)

- [Implement Repository Base and Unit of Work in C#](https://dev.to/1001binary/implement-repository-base-and-unit-of-work-in-c-2ncg)

- [Repository Pattern C# ultimate guide: Entity Framework Core, Clean Architecture, DTOs, Dependency Injection, CQRS](https://medium.com/@codebob75/repository-pattern-c-ultimate-guide-entity-framework-core-clean-architecture-dtos-dependency-6a8d8b444dcb)

- [Implementing ASP.NET CRUD APIs with Repository Pattern and Unit of Work](https://medium.com/@tahatasleem01/implementing-asp-net-crud-apis-with-repository-pattern-and-unit-of-work-b34a86d91baf)

- [A Comprehensive Guide to Repository Pattern in .NET: Implementation and Best Practices](https://medium.com/@dhananjay_1891/a-comprehensive-guide-to-repository-pattern-in-net-implementation-and-best-practices-d67c3a92e618)

#### 21). Singleton Design Pattern

- 

#### 22). REST Api. How to create REST API?

🎮 You can implement a matchmaking service using REST APIs or SignalR to find and assign players to games based on their skills, region, or preferences.

- [How To Build a RESTful API with ASP.NET Core](https://medium.com/net-core/how-to-build-a-restful-api-with-asp-net-core-fb7dd8d3e5e3)

- [Create rest API in .Net Core](https://medium.com/@sagarkumar2499/create-rest-api-in-net-core-b2aed00416fd)

#### 23). What are HTTP Verbs?

- 

#### 24). What is Pagination?

- 

#### 25). What is Data Annotations(Validations)? Client Side and Server Side Validations.

- 

#### 26). Unit Testing - NUnit and XUnit

- [Controller Action Return Types in ASP.NET Core Web API](https://dotnettutorials.net/lesson/controller-action-return-types-core-web-api/)


  ## Game Server using Dot Net Core




  ## Minor Projects

#### 1). CRUD Operations

- [ASP.NET Core Web Application](https://www.youtube.com/watch?v=T-e554Zt3n4)

- [CRUD Operations using ASP.NET Core MVC](https://www.youtube.com/watch?v=SfWuOFEatYc)

#### 2). Custom Identity

- [Custom Identity in Asp.Net Core MVC](https://www.youtube.com/watch?v=93ssXlCPcuI&t=2158s)

## 0). Advanced C# Concepts

- ▶️ [Advanced C# Topics](https://www.youtube.com/watch?v=VT9ueWBqquU&list=PLwhVruPHD9ryiH4kN0EHYeXQXIOHLBcJX&index=1)

## ASP.NET MVC

- ▶️ [Learn ASP.NET MVC (.NET 6)](https://www.youtube.com/watch?v=H14S7x8q_vQ&list=PLqVWQ84m1Q7EiKKyOpiWSVcpG3qUmJ0Xc&index=1)

- ▶️ [Full Course - Learn ASP.NET Core MVC in .NET 8 | CRUD Operations](https://www.youtube.com/watch?v=BzlPrVB_DwA)

## Best Channels PlayLists

- ▶️ [Code Unparalleled .NET Playlist](https://www.youtube.com/@CodeUnparalleled/playlists)








 
