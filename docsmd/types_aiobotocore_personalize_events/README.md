# PersonalizeEvents module

> [Index](../README.md) > PersonalizeEvents


!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `PersonalizeEvents` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[personalize-events]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[personalize-events]'


# standalone installation
python -m pip install types-aiobotocore-personalize-events
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-personalize-events
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PersonalizeEventsClient

Type annotations and code completion for  `#!python session.create_client("personalize-events")` as [PersonalizeEventsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize_events.client import PersonalizeEventsClient


session = get_session()
async with session.create_client("personalize-events") as client:
    client: PersonalizeEventsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_personalize_events.literals import PersonalizeEventsServiceName

def get_value() -> PersonalizeEventsServiceName:
    return "personalize-events"
```

- [PersonalizeEventsServiceName](./literals.md#personalizeeventsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_personalize_events.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [PutEventsRequestRequestTypeDef](./type_defs.md#puteventsrequestrequesttypedef)
- [PutItemsRequestRequestTypeDef](./type_defs.md#putitemsrequestrequesttypedef)
- [PutUsersRequestRequestTypeDef](./type_defs.md#putusersrequestrequesttypedef)

