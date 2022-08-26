# ivschat module

> [Index](../README.md) > ivschat


!!! note ""

    Auto-generated documentation for [ivschat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
    type annotations stubs module [types-aiobotocore-ivschat](https://pypi.org/project/types-aiobotocore-ivschat/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ivschat` service.

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

## ivschatClient

Type annotations and code completion for  `#!python session.create_client("ivschat")` as [ivschatClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ivschat.client import ivschatClient


session = get_session()
async with session.create_client("ivschat") as client:
    client: ivschatClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_ivschat.literals import ChatTokenCapabilityType

def get_value() -> ChatTokenCapabilityType:
    return "DELETE_MESSAGE"
```

- [ChatTokenCapabilityType](./literals.md#chattokencapabilitytype)
- [FallbackResultType](./literals.md#fallbackresulttype)
- [ivschatServiceName](./literals.md#ivschatservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_ivschat.type_defs import CreateChatTokenRequestRequestTypeDef

def get_value() -> CreateChatTokenRequestRequestTypeDef:
    return {
        "roomIdentifier": ...,
        "userId": ...,
    }
```

- [CreateChatTokenRequestRequestTypeDef](./type_defs.md#createchattokenrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef)
- [DeleteMessageRequestRequestTypeDef](./type_defs.md#deletemessagerequestrequesttypedef)
- [DeleteRoomRequestRequestTypeDef](./type_defs.md#deleteroomrequestrequesttypedef)
- [DisconnectUserRequestRequestTypeDef](./type_defs.md#disconnectuserrequestrequesttypedef)
- [GetRoomRequestRequestTypeDef](./type_defs.md#getroomrequestrequesttypedef)
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
- [ListRoomsResponseTypeDef](./type_defs.md#listroomsresponsetypedef)

