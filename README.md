# dot-net-core-centos-7
Runnig .net core on centos 7

First steps
- vagrant up base-centos-7

Install .NET Core for CentOS 7.1 based on https://www.microsoft.com/net/core#centos

I did : 
- `curl -sSL https://raw.githubusercontent.com/dotnet/cli/rel/1.0.0-preview1/scripts/obtain/dotnet-install.sh | bash /dev/stdin --version 1.0.0-preview1-002702 --install-dir ~/dotnet`

Then I got following error:
`dotnet_install: Error: Unable to locate libunwind. Install libunwind to continue`
`dotnet_install: Error: Unable to locate libicu. Install libicu to continue`

I did:
- `yum update`
- `yum install libunwind`
- `yum install libicu`
- `curl -sSL https://raw.githubusercontent.com/dotnet/cli/rel/1.0.0-preview1/scripts/obtain/dotnet-install.sh | bash /dev/stdin --version 1.0.0-preview1-002702 --install-dir ~/dotnet`
- `sudo ln -s ~/dotnet/dotnet /usr/bin`

.Net core is now installed on the centos 7 machine
