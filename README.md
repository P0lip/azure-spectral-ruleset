# Azure Spectral Ruleset

This repository contains a [Spectral](https://github.com/stoplightio/spectral) ruleset to check conformance
to the [Azure API Guidelines](https://github.com/microsoft/api-guidelines/blob/vNext/azure/Guidelines.md) and
the [Azure OpenAPI Style Guidelines](./openapi-style-guidelines.md).

## How to use

### Install Spectral

`npm install -g @stoplightio/spectral`

### Usage

You can specify the ruleset directly on the command line:

`spectral lint -r https://raw.githubusercontent.com/mkistler/azure-spectral-ruleset/main/spectral.yaml <api definition file>`

Or you can create a Spectral configuration file (`.spectral.yaml`) that references the ruleset:

```yaml
extends:
  - https://raw.githubusercontent.com/mkistler/azure-spectral-ruleset/main/spectral.yaml
```

### Example

```bash
spectral lint -r https://raw.githubusercontent.com/mkistler/azure-spectral-ruleset/main/spectral.yaml petstore.yaml
```

## Contributing

This project welcomes contributions and suggestions. Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.microsoft.com.

When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.