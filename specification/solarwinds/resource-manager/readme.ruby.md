## Ruby

These settings apply only when `--ruby` is specified on the command line.

```yaml
package-name: azure_mgmt_solarwinds
package-version: 2023-01-01-preview
azure-arm: true
```

### Tag: package-2023-01-01-preview and ruby

These settings apply only when `--tag=package-2023-01-01-preview --ruby` is specified on the command line.
Please also specify `--ruby-sdks-folder=<path to the root directory of your azure-sdk-for-ruby clone>`.

```yaml $(tag) == 'package-2023-01-01-preview' && $(ruby)
namespace: SolarWinds.Observability
output-folder: $(ruby-sdks-folder)/solarwinds
```