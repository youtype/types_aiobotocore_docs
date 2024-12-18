# Ivschat module

> [Index](../README.md) > Ivschat


!!! note ""

    Auto-generated documentation for [Ivschat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
    type annotations stubs module [types-aiobotocore-ivschat](https://pypi.org/project/types-aiobotocore-ivschat/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Ivschat` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Ivschat` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ivschat]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ivschat]'

# standalone installation
python -m pip install types-aiobotocore-ivschat
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ivschat
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IvschatClient

Type annotations and code completion for  `#!python session.create_client("ivschat")` as [IvschatClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#Ivschat.Client)

```python
# IvschatClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ivschat.client import IvschatClient


session = get_session()
async with session.create_client("ivschat") as client:
    client: IvschatClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ChatTokenCapabilityType usage example

from types_aiobotocore_ivschat.literals import ChatTokenCapabilityType

def get_value() -> ChatTokenCapabilityType:
    return "DELETE_MESSAGE"
```

- [ChatTokenCapabilityType](./literals.md#chattokencapabilitytype)
- [CreateLoggingConfigurationStateType](./literals.md#createloggingconfigurationstatetype)
- [FallbackResultType](./literals.md#fallbackresulttype)
- [LoggingConfigurationStateType](./literals.md#loggingconfigurationstatetype)
- [UpdateLoggingConfigurationStateType](./literals.md#updateloggingconfigurationstatetype)
- [IvschatServiceName](./literals.md#ivschatservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CloudWatchLogsDestinationConfigurationTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigurationtypedef)
- [CreateChatTokenRequestRequestTypeDef](./type_defs.md#createchattokenrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef)
- [DeleteLoggingConfigurationRequestRequestTypeDef](./type_defs.md#deleteloggingconfigurationrequestrequesttypedef)
- [DeleteMessageRequestRequestTypeDef](./type_defs.md#deletemessagerequestrequesttypedef)
- [DeleteRoomRequestRequestTypeDef](./type_defs.md#deleteroomrequestrequesttypedef)
- [FirehoseDestinationConfigurationTypeDef](./type_defs.md#firehosedestinationconfigurationtypedef)
- [S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef)
- [DisconnectUserRequestRequestTypeDef](./type_defs.md#disconnectuserrequestrequesttypedef)
- [GetLoggingConfigurationRequestRequestTypeDef](./type_defs.md#getloggingconfigurationrequestrequesttypedef)
- [GetRoomRequestRequestTypeDef](./type_defs.md#getroomrequestrequesttypedef)
- [ListLoggingConfigurationsRequestRequestTypeDef](./type_defs.md#listloggingconfigurationsrequestrequesttypedef)
- [ListRoomsRequestRequestTypeDef](./type_defs.md#listroomsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [SendEventRequestRequestTypeDef](./type_defs.md#sendeventrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateChatTokenResponseTypeDef](./type_defs.md#createchattokenresponsetypedef)
- [DeleteMessageResponseTypeDef](./type_defs.md#deletemessageresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [SendEventResponseTypeDef](./type_defs.md#sendeventresponsetypedef)
- [CreateRoomRequestRequestTypeDef](./type_defs.md#createroomrequestrequesttypedef)
- [CreateRoomResponseTypeDef](./type_defs.md#createroomresponsetypedef)
- [GetRoomResponseTypeDef](./type_defs.md#getroomresponsetypedef)
- [RoomSummaryTypeDef](./type_defs.md#roomsummarytypedef)
- [UpdateRoomRequestRequestTypeDef](./type_defs.md#updateroomrequestrequesttypedef)
- [UpdateRoomResponseTypeDef](./type_defs.md#updateroomresponsetypedef)
- [DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef)
- [ListRoomsResponseTypeDef](./type_defs.md#listroomsresponsetypedef)
- [CreateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#createloggingconfigurationrequestrequesttypedef)
- [CreateLoggingConfigurationResponseTypeDef](./type_defs.md#createloggingconfigurationresponsetypedef)
- [GetLoggingConfigurationResponseTypeDef](./type_defs.md#getloggingconfigurationresponsetypedef)
- [LoggingConfigurationSummaryTypeDef](./type_defs.md#loggingconfigurationsummarytypedef)
- [UpdateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#updateloggingconfigurationrequestrequesttypedef)
- [UpdateLoggingConfigurationResponseTypeDef](./type_defs.md#updateloggingconfigurationresponsetypedef)
- [ListLoggingConfigurationsResponseTypeDef](./type_defs.md#listloggingconfigurationsresponsetypedef)

