# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for Pip.Services 1.0 Archive

This is a workspace for [Pip.Services Archive 1.0](https://github.com/pip-services-archive).
It is obsolete and being replaced by [Pip.Services](https://github.com/pip-services/pip-services)

The workspace enables build, test, and release across the following projects:

- **pip-services-devenv** - Development environment with infrastructure services
- **pip-services-runtime-node** - Microservices runtime in Node.js
- **pip-services-runtime-dotnet** - Microservices runtime in .NET
- **pip-services-runtime-java** - Microservices runtime in Java
- **pip-services-runtime-go** - Microservices runtime in Go
- **pip-services-runtime-python** - Microservices runtime in Python
- **pip-services-test-node** - Microservices testing framework in Node.js
- **pip-services-template-node** - Microservice template in Node.js
- **pip-services-template-dotnet** - Microservice template in .NET
- **pip-services-template-java** - Microservice template in Java
- **pip-services-template-go** - Microservice template in Go
- **pip-services-template-python** - Microservice template in Python

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services-archive/pip-services-archive-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop infrastructure services
```bash
> piptask start -component pip-services-devenv
> piptask stop -component pip-services-devenv
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The 1.0 version of Pip.Services is created by:
- **Volodymyr Tkachenko**
- **Sergey Seroukhov**
- **Mark Zontak**
