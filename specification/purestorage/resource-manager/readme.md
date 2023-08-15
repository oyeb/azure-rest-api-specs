# PureStorage.Block

> see https://aka.ms/autorest

This is the AutoRest configuration file for PureStorage.Block.

## Getting Started

To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:

> `autorest readme.md`

To see additional help and options, run:

> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration

### Basic Information

These are the global settings for the PureStorage.Block.

```yaml
openapi-type: arm
openapi-subtype: rpaas
tag: package-2023-06-01-preview
```

### Tag: package-2023-06-01-preview

These settings apply only when `--tag=package-2023-06-01-preview` is specified on the command line.

```yaml $(tag) == 'package-2023-06-01-preview'
input-file:
  - PureStorage.Block/preview/2023-06-01-preview/purestorage.json
```