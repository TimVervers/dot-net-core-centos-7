# dot-net-core-centos-7
Runnig .NET core

# CentOS 7

Install .NET Core for CentOS 7.1 based on https://www.microsoft.com/net/core#centos

- `yum update`
- `yum install libunwind`
- `yum install libicu`
- `curl -sSL https://raw.githubusercontent.com/dotnet/cli/rel/1.0.0-preview1/scripts/obtain/dotnet-install.sh | bash /dev/stdin --version 1.0.0-preview1-002702 --install-dir ~/dotnet`
- `sudo ln -s ~/dotnet/dotnet /usr/bin`

.NET core is now installed on the centos 7 machine!

# OSX

Install .NET Core for OXS based on https://www.microsoft.com/net/core#macosx

- Install brew
- `brew update`
- `brew install openssl`
- `brew link --force openssl`

# Running the app
- `dotnet restore`
- `dotnet run --server.urls=http://localhost:5000/` (You can specify all hostnames/ips/ports)
