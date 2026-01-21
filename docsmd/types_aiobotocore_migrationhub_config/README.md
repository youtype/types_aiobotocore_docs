# MigrationHubConfig module

> [Index](../README.md) > MigrationHubConfig


!!! note ""

    Auto-generated documentation for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#migrationhubconfig)
    type annotations stubs module [types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MigrationHubConfig` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MigrationHubConfig` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[migrationhub-config]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[migrationhub-config]'

# standalone installation
python -m pip install types-aiobotocore-migrationhub-config
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-migrationhub-config
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MigrationHubConfigClient

Type annotations and code completion for  `#!python session.create_client("migrationhub-config")` as [MigrationHubConfigClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client)

```python
# MigrationHubConfigClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient


session = get_session()
async with session.create_client("migrationhub-config") as client:
    client: MigrationHubConfigClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# TargetTypeType usage example

from types_aiobotocore_migrationhub_config.literals import TargetTypeType

def get_value() -> TargetTypeType:
    return "ACCOUNT"
```

- [TargetTypeType](./literals.md#targettypetype)
- [MigrationHubConfigServiceName](./literals.md#migrationhubconfigservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TargetTypeDef](./type_defs.md#targettypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteHomeRegionControlRequestTypeDef](./type_defs.md#deletehomeregioncontrolrequesttypedef)
- [CreateHomeRegionControlRequestTypeDef](./type_defs.md#createhomeregioncontrolrequesttypedef)
- [DescribeHomeRegionControlsRequestTypeDef](./type_defs.md#describehomeregioncontrolsrequesttypedef)
- [HomeRegionControlTypeDef](./type_defs.md#homeregioncontroltypedef)
- [GetHomeRegionResultTypeDef](./type_defs.md#gethomeregionresulttypedef)
- [CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef)
- [DescribeHomeRegionControlsResultTypeDef](./type_defs.md#describehomeregioncontrolsresulttypedef)

