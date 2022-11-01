# Cognitive Services Anomaly Detector SDK

> see https://aka.ms/autorest

Configuration for generating Anomaly Detector SDK.

The current release is `release_1_1`.

``` yaml
tag: release_1_1
add-credentials: true
openapi-type: data-plane
```

# Releases

### Release 1.0
These settings apply only when `--tag=release_1_0` is specified on the command line.

``` yaml $(tag) == 'release_1_0'
input-file: stable/v1.0/AnomalyDetector.json
```

### Release 1.1-preview
These settings apply only when `--tag=release_1_1_preview` is specified on the command line.

``` yaml $(tag) == 'release_1_1_preview'
input-file: 
  - preview/v1.1-preview/AnomalyDetector.json
  - preview/v1.1-preview/MultivariateAnomalyDetector.json
```

### Release 1.1-preview.1
These settings apply only when `--tag=release_1_1_preview.1` is specified on the command line.

``` yaml $(tag) == 'release_1_1_preview.1'
input-file: 
  - preview/v1.1-preview.1/AnomalyDetector.json
  - preview/v1.1-preview.1/MultivariateAnomalyDetector.json
```

### Release 1.1-preview.2
These settings apply only when `--tag=release_1_1_preview.2` is specified on the command line.

```yaml $(tag) == 'release_1_1_preview.2'
input-file:
  - preview/v1.1-preview.2/AnomalyDetector.json
  - preview/v1.1-preview.2/MultivariateAnomalyDetector.json
  - preview/v1.1-preview.2/RootCauseAnalysis.json
```

### Release 1.1
These settings apply only when `--tag=release_1_1` is specified on the command line.

```yaml $(tag) == 'release_1_1'
input-file:
  - stable/v1.1/UnivariateAnomalyDetector.json
  - stable/v1.1/MultivariateAnomalyDetector.json
```

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-net-track2
 ```

## CSharp Settings

These settings apply only when `--csharp` is specified on the command line.

```yaml $(csharp)
sync-methods: None
license-header: MICROSOFT_MIT_NO_VERSION
azure-arm: false
namespace: Microsoft.Azure.CognitiveServices.AnomalyDetector
output-folder: $(csharp-sdks-folder)/cognitiveservices/AnomalyDetector/src/Generated
clear-output-folder: true
```

## Python

See configuration in [readme.python.md](./readme.python.md)

## Go

See configuration in [readme.go.md](./readme.go.md)

## Java

See configuration in [readme.java.md](./readme.java.md)

## Multi-API/Profile support for AutoRest v3 generators 

AutoRest V3 generators require the use of `--tag=all-api-versions` to select api files.

This block is updated by an automatic script. Edits may be lost!

``` yaml $(tag) == 'all-api-versions' /* autogenerated */
# include the azure profile definitions from the standard location
require: $(this-folder)/../../../../profiles/readme.md

# all the input files across all versions
input-file:
  - $(this-folder)/stable/v1.0/AnomalyDetector.json
  - $(this-folder)/stable/v1.1/UnivariateAnomalyDetector.json
  - $(this-folder)/stable/v1.1/MultivariateAnomalyDetector.json
  - $(this-folder)/preview/v1.1-preview/MultivariateAnomalyDetector.json
  - $(this-folder)/preview/v1.1-preview.1/MultivariateAnomalyDetector.json
  - $(this-folder)/preview/v1.1-preview.2/AnomalyDetector.json
  - $(this-folder)/preview/v1.1-preview.2/MultivariateAnomalyDetector.json
  - $(this-folder)/preview/v1.1-preview.2/RootCauseAnalysis.json
```

If there are files that should not be in the `all-api-versions` set, 
uncomment the  `exclude-file` section below and add the file paths.

``` yaml $(tag) == 'all-api-versions'
#exclude-file: 
#  - $(this-folder)/Microsoft.Example/stable/2010-01-01/somefile.json
```
