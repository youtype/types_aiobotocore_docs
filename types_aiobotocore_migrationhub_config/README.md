<a id="type-annotations-for-aiobotocore-migrationhubconfig-module"></a>

# Type annotations for aiobotocore MigrationHubConfig module

> [Index](..) > MigrationHubConfig

Auto-generated documentation for
[MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
type annotations stubs module
[types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

- [Type annotations for aiobotocore MigrationHubConfig module](#type-annotations-for-aiobotocore-migrationhubconfig-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [MigrationHubConfigClient](#migrationhubconfigclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `MigrationHubConfig`.

<a id="from-pypi-with-pip"></a>

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

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-migrationhub-config
```

<a id="migrationhubconfigclient"></a>

## MigrationHubConfigClient

Type annotations for `session.create_client("migrationhub-config")` as
[MigrationHubConfigClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [create_home_region_control](./client.md#create_home_region_control)
- [describe_home_region_controls](./client.md#describe_home_region_controls)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_home_region](./client.md#get_home_region)

<a id="exceptions"></a>

### Exceptions

MigrationHubConfigClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- DryRunOperation
- InternalServerError
- InvalidInputException
- ServiceUnavailableException
- ThrottlingException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_migrationhub_config.literals import TargetTypeType, ...
```

- [TargetTypeType](./literals.md#targettypetype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_migrationhub_config.type_defs import CreateHomeRegionControlRequestRequestTypeDef, ...
```

- [CreateHomeRegionControlRequestRequestTypeDef](./type_defs.md#createhomeregioncontrolrequestrequesttypedef)
- [CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef)
- [DescribeHomeRegionControlsRequestRequestTypeDef](./type_defs.md#describehomeregioncontrolsrequestrequesttypedef)
- [DescribeHomeRegionControlsResultTypeDef](./type_defs.md#describehomeregioncontrolsresulttypedef)
- [GetHomeRegionResultTypeDef](./type_defs.md#gethomeregionresulttypedef)
- [HomeRegionControlTypeDef](./type_defs.md#homeregioncontroltypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TargetTypeDef](./type_defs.md#targettypedef)
