# RickrollingMiddleware

![CI](https://github.com/ThomasArdal/RickrollingMiddleware/workflows/CI/badge.svg)
[![Nuget](https://img.shields.io/nuget/v/RickrollingMiddleware)](https://www.nuget.org/packages/RickrollingMiddleware/)

This package implements a piece of ASP.NET Core middleware, rick rolling anyone requesting invalid URLs. The code is inspired by this tweet:

> 🙃 Make sure to rickroll people trying to break into your site <a href="https://t.co/4cd80Pr9p9">pic.twitter.com/4cd80Pr9p9</a></p>&mdash; Liam Hammett (@LiamHammett) <a href="https://twitter.com/LiamHammett/status/1260984553570570240?ref_src=twsrc%5Etfw">May 14, 2020</a>

## Usage

Install the `RickrollingMiddleware` NuGet package:

```powershell
PM> Install-Package RickrollingMiddleware
```

Call `UseRickrolling` in the `Configure` method:

```csharp
public void Configure(IApplicationBuilder app, IWebHostEnvironment env)
{
    // ...

    app.UseRickrolling();

    // ...
}
```
