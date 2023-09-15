# AppSecurity

> see https://aka.ms/autorest

This is the AutoRest configuration file for AppSecurity.

---

## Getting Started

To build the SDK for AppSecurity, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`

---

## Configuration

### Basic Information

These are the global settings for the AppSecurity API.

```yaml
title: appsecurityClient
openapi-type: arm
openapi-subtype: rpaas
tag: package-2023-02-06-preview
```

### Tag: package-2023-02-06-preview

These settings apply only when `--tag=package-2023-02-06-preview` is specified on the command line.

```yaml $(tag) == 'package-package-2023-02-06-preview'
input-file:
    - Microsoft.AppSecurity/preview/2023-02-06-preview/AppSecurity.json
```

---

# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

```yaml $(swagger-to-sdk)
swagger-to-sdk:
    - repo: azure-sdk-for-python-track2
    - repo: azure-sdk-for-java
    - repo: azure-sdk-for-go
    - repo: azure-sdk-for-net-track2
    - repo: azure-sdk-for-js
    - repo: azure-sdk-for-node
    - repo: azure-sdk-for-ruby
    - repo: azure-resource-manager-schemas
    - repo: azure-powershell
```

## Az

See configuration in [readme.az.md](./readme.az.md)

## Go

See configuration in [readme.go.md](./readme.go.md)

## Python

See configuration in [readme.python.md](./readme.python.md)

## TypeScript

See configuration in [readme.typescript.md](./readme.typescript.md)

## CSharp

See configuration in [readme.csharp.md](./readme.csharp.md)