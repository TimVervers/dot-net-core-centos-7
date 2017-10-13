# dot-net-core-centos-7
Runnig .NET core

# CentOS 7

## .NET Core 2.0

Install .NET Core 2.0 for CentOS 7 based on https://github.com/dotnet/source-build

- `yum install centos-release-dotnet`
- `yum install rh-dotnet20`

.NET Core 2.0 is now installed on the CentOS 7 machine! To use it:

- `scl enable rh-dotnet20 bash`
- `dotnet --info`

## .NET Core 1.1

Install .NET Core 1.1 for CentOS 7

- `yum install centos-release-dotnet`
- `yum install rh-dotnetcore11`

.NET Core 1.1 is now installed on the CentOS 7 machine! To use it:

- `scl enable rh-dotnetcore11 bash`
- `dotnet --info`

## .NET Core 1.0

Install .NET Core 1.0 for CentOS 7

- `yum install centos-release-dotnet`
- `yum install rh-dotnetcore10`

.NET Core 1.0 is now installed on the CentOS 7 machine! To use it:

- `scl enable rh-dotnetcore10 bash`
- `dotnet --info`

# OSX

Install .NET Core for OXS based on https://www.microsoft.com/net/core#macosx

- Install brew
- `brew update`
- `brew install openssl`
- `brew link --force openssl`

# Running the app
- `dotnet restore`
- `dotnet run --server.urls=http://localhost:5000/` (You can specify all hostnames/ips/ports)
