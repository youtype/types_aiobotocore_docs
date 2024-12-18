# ChimeSDKIdentity module

> [Index](../README.md) > ChimeSDKIdentity


!!! note ""

    Auto-generated documentation for [ChimeSDKIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#chimesdkidentity)
    type annotations stubs module [types-aiobotocore-chime-sdk-identity](https://pypi.org/project/types-aiobotocore-chime-sdk-identity/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ChimeSDKIdentity` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ChimeSDKIdentity` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[chime-sdk-identity]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[chime-sdk-identity]'

# standalone installation
python -m pip install types-aiobotocore-chime-sdk-identity
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-chime-sdk-identity
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ChimeSDKIdentityClient

Type annotations and code completion for  `#!python session.create_client("chime-sdk-identity")` as [ChimeSDKIdentityClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client)

```python
# ChimeSDKIdentityClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_identity.client import ChimeSDKIdentityClient


session = get_session()
async with session.create_client("chime-sdk-identity") as client:
    client: ChimeSDKIdentityClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AllowMessagesType usage example

from types_aiobotocore_chime_sdk_identity.literals import AllowMessagesType

def get_value() -> AllowMessagesType:
    return "ALL"
```

- [AllowMessagesType](./literals.md#allowmessagestype)
- [AppInstanceUserEndpointTypeType](./literals.md#appinstanceuserendpointtypetype)
- [EndpointStatusReasonType](./literals.md#endpointstatusreasontype)
- [EndpointStatusType](./literals.md#endpointstatustype)
- [ExpirationCriterionType](./literals.md#expirationcriteriontype)
- [RespondsToType](./literals.md#respondstotype)
- [StandardMessagesType](./literals.md#standardmessagestype)
- [TargetedMessagesType](./literals.md#targetedmessagestype)
- [ChimeSDKIdentityServiceName](./literals.md#chimesdkidentityservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [AppInstanceBotSummaryTypeDef](./type_defs.md#appinstancebotsummarytypedef)
- [ChannelRetentionSettingsTypeDef](./type_defs.md#channelretentionsettingstypedef)
- [AppInstanceSummaryTypeDef](./type_defs.md#appinstancesummarytypedef)
- [AppInstanceTypeDef](./type_defs.md#appinstancetypedef)
- [EndpointStateTypeDef](./type_defs.md#endpointstatetypedef)
- [EndpointAttributesTypeDef](./type_defs.md#endpointattributestypedef)
- [AppInstanceUserSummaryTypeDef](./type_defs.md#appinstanceusersummarytypedef)
- [ExpirationSettingsTypeDef](./type_defs.md#expirationsettingstypedef)
- [CreateAppInstanceAdminRequestRequestTypeDef](./type_defs.md#createappinstanceadminrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteAppInstanceAdminRequestRequestTypeDef](./type_defs.md#deleteappinstanceadminrequestrequesttypedef)
- [DeleteAppInstanceBotRequestRequestTypeDef](./type_defs.md#deleteappinstancebotrequestrequesttypedef)
- [DeleteAppInstanceRequestRequestTypeDef](./type_defs.md#deleteappinstancerequestrequesttypedef)
- [DeleteAppInstanceUserRequestRequestTypeDef](./type_defs.md#deleteappinstanceuserrequestrequesttypedef)
- [DeregisterAppInstanceUserEndpointRequestRequestTypeDef](./type_defs.md#deregisterappinstanceuserendpointrequestrequesttypedef)
- [DescribeAppInstanceAdminRequestRequestTypeDef](./type_defs.md#describeappinstanceadminrequestrequesttypedef)
- [DescribeAppInstanceBotRequestRequestTypeDef](./type_defs.md#describeappinstancebotrequestrequesttypedef)
- [DescribeAppInstanceRequestRequestTypeDef](./type_defs.md#describeappinstancerequestrequesttypedef)
- [DescribeAppInstanceUserEndpointRequestRequestTypeDef](./type_defs.md#describeappinstanceuserendpointrequestrequesttypedef)
- [DescribeAppInstanceUserRequestRequestTypeDef](./type_defs.md#describeappinstanceuserrequestrequesttypedef)
- [GetAppInstanceRetentionSettingsRequestRequestTypeDef](./type_defs.md#getappinstanceretentionsettingsrequestrequesttypedef)
- [InvokedByTypeDef](./type_defs.md#invokedbytypedef)
- [ListAppInstanceAdminsRequestRequestTypeDef](./type_defs.md#listappinstanceadminsrequestrequesttypedef)
- [ListAppInstanceBotsRequestRequestTypeDef](./type_defs.md#listappinstancebotsrequestrequesttypedef)
- [ListAppInstanceUserEndpointsRequestRequestTypeDef](./type_defs.md#listappinstanceuserendpointsrequestrequesttypedef)
- [ListAppInstanceUsersRequestRequestTypeDef](./type_defs.md#listappinstanceusersrequestrequesttypedef)
- [ListAppInstancesRequestRequestTypeDef](./type_defs.md#listappinstancesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAppInstanceRequestRequestTypeDef](./type_defs.md#updateappinstancerequestrequesttypedef)
- [UpdateAppInstanceUserEndpointRequestRequestTypeDef](./type_defs.md#updateappinstanceuserendpointrequestrequesttypedef)
- [UpdateAppInstanceUserRequestRequestTypeDef](./type_defs.md#updateappinstanceuserrequestrequesttypedef)
- [AppInstanceAdminSummaryTypeDef](./type_defs.md#appinstanceadminsummarytypedef)
- [AppInstanceAdminTypeDef](./type_defs.md#appinstanceadmintypedef)
- [AppInstanceRetentionSettingsTypeDef](./type_defs.md#appinstanceretentionsettingstypedef)
- [AppInstanceUserEndpointSummaryTypeDef](./type_defs.md#appinstanceuserendpointsummarytypedef)
- [AppInstanceUserEndpointTypeDef](./type_defs.md#appinstanceuserendpointtypedef)
- [RegisterAppInstanceUserEndpointRequestRequestTypeDef](./type_defs.md#registerappinstanceuserendpointrequestrequesttypedef)
- [AppInstanceUserTypeDef](./type_defs.md#appinstanceusertypedef)
- [PutAppInstanceUserExpirationSettingsRequestRequestTypeDef](./type_defs.md#putappinstanceuserexpirationsettingsrequestrequesttypedef)
- [CreateAppInstanceAdminResponseTypeDef](./type_defs.md#createappinstanceadminresponsetypedef)
- [CreateAppInstanceBotResponseTypeDef](./type_defs.md#createappinstancebotresponsetypedef)
- [CreateAppInstanceResponseTypeDef](./type_defs.md#createappinstanceresponsetypedef)
- [CreateAppInstanceUserResponseTypeDef](./type_defs.md#createappinstanceuserresponsetypedef)
- [DescribeAppInstanceResponseTypeDef](./type_defs.md#describeappinstanceresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListAppInstanceBotsResponseTypeDef](./type_defs.md#listappinstancebotsresponsetypedef)
- [ListAppInstanceUsersResponseTypeDef](./type_defs.md#listappinstanceusersresponsetypedef)
- [ListAppInstancesResponseTypeDef](./type_defs.md#listappinstancesresponsetypedef)
- [PutAppInstanceUserExpirationSettingsResponseTypeDef](./type_defs.md#putappinstanceuserexpirationsettingsresponsetypedef)
- [RegisterAppInstanceUserEndpointResponseTypeDef](./type_defs.md#registerappinstanceuserendpointresponsetypedef)
- [UpdateAppInstanceBotResponseTypeDef](./type_defs.md#updateappinstancebotresponsetypedef)
- [UpdateAppInstanceResponseTypeDef](./type_defs.md#updateappinstanceresponsetypedef)
- [UpdateAppInstanceUserEndpointResponseTypeDef](./type_defs.md#updateappinstanceuserendpointresponsetypedef)
- [UpdateAppInstanceUserResponseTypeDef](./type_defs.md#updateappinstanceuserresponsetypedef)
- [CreateAppInstanceRequestRequestTypeDef](./type_defs.md#createappinstancerequestrequesttypedef)
- [CreateAppInstanceUserRequestRequestTypeDef](./type_defs.md#createappinstanceuserrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [LexConfigurationTypeDef](./type_defs.md#lexconfigurationtypedef)
- [ListAppInstanceAdminsResponseTypeDef](./type_defs.md#listappinstanceadminsresponsetypedef)
- [DescribeAppInstanceAdminResponseTypeDef](./type_defs.md#describeappinstanceadminresponsetypedef)
- [GetAppInstanceRetentionSettingsResponseTypeDef](./type_defs.md#getappinstanceretentionsettingsresponsetypedef)
- [PutAppInstanceRetentionSettingsRequestRequestTypeDef](./type_defs.md#putappinstanceretentionsettingsrequestrequesttypedef)
- [PutAppInstanceRetentionSettingsResponseTypeDef](./type_defs.md#putappinstanceretentionsettingsresponsetypedef)
- [ListAppInstanceUserEndpointsResponseTypeDef](./type_defs.md#listappinstanceuserendpointsresponsetypedef)
- [DescribeAppInstanceUserEndpointResponseTypeDef](./type_defs.md#describeappinstanceuserendpointresponsetypedef)
- [DescribeAppInstanceUserResponseTypeDef](./type_defs.md#describeappinstanceuserresponsetypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [AppInstanceBotTypeDef](./type_defs.md#appinstancebottypedef)
- [CreateAppInstanceBotRequestRequestTypeDef](./type_defs.md#createappinstancebotrequestrequesttypedef)
- [UpdateAppInstanceBotRequestRequestTypeDef](./type_defs.md#updateappinstancebotrequestrequesttypedef)
- [DescribeAppInstanceBotResponseTypeDef](./type_defs.md#describeappinstancebotresponsetypedef)

