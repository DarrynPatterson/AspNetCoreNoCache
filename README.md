# AspNetCoreNoCache

The [AspNetCoreNoCache package](https://www.nuget.org/packages/AspNetCoreNoCache/) is an ASP.NET Core solution which ensures that http responses are not cached.

[![NuGet](https://img.shields.io/nuget/v/AspNetCoreNoCache.svg?maxAge=259200)](https://www.nuget.org/packages/AspNetCoreNoCache/) 

**NuGet install:**

Install-Package AspNetCoreNoCache

**Startup.cs code:**

    public void Configure(IApplicationBuilder app)
    {
        app.UseMiddleware<NoCacheMiddleware>();
    }