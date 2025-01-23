# SupportApp module

> [Index](../README.md) > SupportApp


!!! note ""

    Auto-generated documentation for [SupportApp](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#supportapp)
    type annotations stubs module [types-aiobotocore-support-app](https://pypi.org/project/types-aiobotocore-support-app/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SupportApp` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SupportApp` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[support-app]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[support-app]'

# standalone installation
python -m pip install types-aiobotocore-support-app
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-support-app
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SupportAppClient

Type annotations and code completion for  `#!python session.create_client("support-app")` as [SupportAppClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp.Client)

```python
# SupportAppClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_support_app.client import SupportAppClient


session = get_session()
async with session.create_client("support-app") as client:
    client: SupportAppClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountTypeType usage example

from types_aiobotocore_support_app.literals import AccountTypeType

def get_value() -> AccountTypeType:
    return "management"
```

- [AccountTypeType](./literals.md#accounttypetype)
- [NotificationSeverityLevelType](./literals.md#notificationseverityleveltype)
- [SupportAppServiceName](./literals.md#supportappservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CreateSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#createslackchannelconfigurationrequestrequesttypedef)
- [DeleteSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#deleteslackchannelconfigurationrequestrequesttypedef)
- [DeleteSlackWorkspaceConfigurationRequestRequestTypeDef](./type_defs.md#deleteslackworkspaceconfigurationrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ListSlackChannelConfigurationsRequestRequestTypeDef](./type_defs.md#listslackchannelconfigurationsrequestrequesttypedef)
- [SlackChannelConfigurationTypeDef](./type_defs.md#slackchannelconfigurationtypedef)
- [ListSlackWorkspaceConfigurationsRequestRequestTypeDef](./type_defs.md#listslackworkspaceconfigurationsrequestrequesttypedef)
- [SlackWorkspaceConfigurationTypeDef](./type_defs.md#slackworkspaceconfigurationtypedef)
- [PutAccountAliasRequestRequestTypeDef](./type_defs.md#putaccountaliasrequestrequesttypedef)
- [RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef](./type_defs.md#registerslackworkspacefororganizationrequestrequesttypedef)
- [UpdateSlackChannelConfigurationRequestRequestTypeDef](./type_defs.md#updateslackchannelconfigurationrequestrequesttypedef)
- [GetAccountAliasResultTypeDef](./type_defs.md#getaccountaliasresulttypedef)
- [RegisterSlackWorkspaceForOrganizationResultTypeDef](./type_defs.md#registerslackworkspacefororganizationresulttypedef)
- [UpdateSlackChannelConfigurationResultTypeDef](./type_defs.md#updateslackchannelconfigurationresulttypedef)
- [ListSlackChannelConfigurationsResultTypeDef](./type_defs.md#listslackchannelconfigurationsresulttypedef)
- [ListSlackWorkspaceConfigurationsResultTypeDef](./type_defs.md#listslackworkspaceconfigurationsresulttypedef)

