# Backend

> **Adopt** - The default choice when selecting technologies
>
> **Assess**  - Technologies that we believe may be valuable, and are currently being assessed to understand their value and impact.
>
> **Hold** - Technologies in hold must no longer be used for new development

## Adopt
### .NET Core LTS
Application development framework. Enables building web applications and APIs with ASP.NET Core.

.NET Core supports cross-platform development end deployment giving us flexibility during development and deployment.

### Web API	
.NET Core component that supports the creation of restful services.

Enables separation of concerns and flexibility when choosing front-end technologies.

### Entity Framework Core	
.NET Core data access technology / ORM

Flexible ORM that can be used with a variety of database providers (SQL Server and In-Memory for testing)

### xUnit	
Unit test framework for the .NET Framework

Out of the box support in all IDEs used by our team (Visual Studio, Visual Studio Code and Rider) and the CI Tool (TeamCity).

Good community support, documentation and compatibility with programming languages and frameworks we use. 

### Varnish	
Used in multiple projects as a caching mechanism.

Use for caching and **not** for routing.

## Assess
### OpenAPI Specification	
Machine-readable interface description for REST APIs

Enables the documentation of APIs, generation / scaffolding of server and clients, and creation mock servers.

Adds flexibility to the development of APIs and increases maintainability of back-end code. Documentation is auto generated and can be in code. Easy to configure.

Recommended by Microsoft in the official Web API documentation.

### Serverless runtimes / Function as a service
Event driven, on-demand running of functions / code. Providers include AWS Lambda, Azure Functions and Google Cloud functions.

Can be used as backend for APIs, data processing, etc.

## Hold
### .NET Framework 4.x	
Application development framework.

Microsoft has shifted focus to .NET Core. The next version - .NET 5 - will be based on .NET Core.

### Internally build frameworks
Examples: NICE.Poe, NICE.Snooze

They decrease maintainability. Consider using already available frameworks or libraries.

### MSpec	
Unit test framework for the .NET Framework.

Used on older projects.

Not as easy to read as NUnit/XUnit. Can cause some clashes with Newtonsoft.json and needs extra plugins to integrate with Resharper. 

### IOC Frameworks	
Castle Windsor, tinyIOC, etc. Used on older projects

Use .NET Core built-in IOC.

### 3rd party ORM frameworks	
simple.data. ORM used with SQL for ISS.

Use Entity Framework. 

### F# for web application development	
Use C#

### NUnit
Unit test framework for the .NET Framework

Out of the box support in all IDEs used by our team (Visual Studio, Visual Studio Code and Rider) and the CI Tool (TeamCity).

Community support has moved to xUnit

