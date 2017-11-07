# MR.AspNet.Identity.EntityFramework6

[![Build status](https://img.shields.io/appveyor/ci/mrahhal/mr-aspnet-identity-entityframework6/master.svg)](https://ci.appveyor.com/project/mrahhal/mr-aspnet-identity-entityframework6)
[![NuGet version](https://badge.fury.io/nu/MR.AspNet.Identity.EntityFramework6.svg)](https://www.nuget.org/packages/MR.AspNet.Identity.EntityFramework6)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

EntityFramework 6 provider + InMemory providers for Asp.Net Core Identity.

## What is this?

All you have to do in your app:

- Remove everything EF Core related, this means: `Microsoft.EntityFrameworkCore.Tools`, `Microsoft.EntityFrameworkCore.SqlServer`, `Microsoft.EntityFrameworkCore.InMemory` and `Microsoft.AspNetCore.Identity.EntityFramework`. And instead add the following: `EntityFramework` and `MR.AspNet.Identity.EntityFramework6`.
- Replace all EF Core namespaces with their EF6 counterparts.

### `MR.AspNet.Identity.EntityFramework6` [![NuGet version](https://badge.fury.io/nu/MR.AspNet.Identity.EntityFramework6.svg)](https://www.nuget.org/packages/MR.AspNet.Identity.EntityFramework6)

The port of `Microsoft.AspNetCore.Identity.EntityFramework` to work under EF6.

### `MR.AspNet.Identity.EntityFramework6.Key.Int` [![NuGet version](https://badge.fury.io/nu/MR.AspNet.Identity.EntityFramework6.Key.Int.svg)](https://www.nuget.org/packages/MR.AspNet.Identity.EntityFramework6.Key.Int)

An implementation that uses an int as the primary key for users and roles.

### `MR.AspNet.Identity.EntityFramework6.InMemory` [![NuGet version](https://badge.fury.io/nu/MR.AspNet.Identity.EntityFramework6.InMemory.svg)](https://www.nuget.org/packages/MR.AspNet.Identity.EntityFramework6.InMemory)

Contains in memory implementations of `IUserStore` and `IRoleStore` to be used in unit tests.

### `MR.AspNet.Identity2.EntityFramework6.InMemory` [![NuGet version](https://badge.fury.io/nu/MR.AspNet.Identity2.EntityFramework6.InMemory.svg)](https://www.nuget.org/packages/MR.AspNet.Identity2.EntityFramework6.InMemory)

Contains in memory implementations of `IUserStore` and `IRoleStore` for identity 2 to be used in unit tests.

**Note:** In memory stores have a dependency on [`MR.Patterns.Repository`](https://github.com/mrahhal/MR.Patterns.Repository) for the in memory repository implementation.

## Samples

Check out the samples in the `samples/` directory.

## EF6 migrations for Asp.Net Core?

Check out [Migrator.EF6](https://github.com/mrahhal/Migrator.EF6).

## Release notes

#### `3.0.2`
- Implement additional interfaces in the stores.

#### `3.0.1`
- Switched to reference `Microsoft.Extensions.Identity.Core`. [#11](https://github.com/mrahhal/MR.AspNet.Identity.EntityFramework6/pull/11)

#### `3.0.0`
- Support Asp.Net Core Identity 2.0.

#### `2.1.0`
This release is for .Net Core 1.1.0
