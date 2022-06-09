# IoTDataPlane module

> [Index](../README.md) > IoTDataPlane


!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `IoTDataPlane`.

### From PyPI with pip

Install `types-aiobotocore` for `IoTDataPlane` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iot-data]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iot-data]'


# standalone installation
python -m pip install types-aiobotocore-iot-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iot-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTDataPlaneClient

Type annotations and code completion for  `#!python session.create_client("iot-data")` as [IoTDataPlaneClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iot_data.client import IoTDataPlaneClient


session = get_session()
async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("iot-data").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator

def get_list_retained_messages_paginator() -> ListRetainedMessagesPaginator:
    return client.get_paginator("list_retained_messages"))
```

- [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iot_data.literals import ListRetainedMessagesPaginatorName

def get_value() -> ListRetainedMessagesPaginatorName:
    return "list_retained_messages"
```

- [ListRetainedMessagesPaginatorName](./literals.md#listretainedmessagespaginatorname)
- [IoTDataPlaneServiceName](./literals.md#iotdataplaneservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iot_data.type_defs import DeleteThingShadowRequestRequestTypeDef

def get_value() -> DeleteThingShadowRequestRequestTypeDef:
    return {
        "thingName": ...,
    }
```

- [DeleteThingShadowRequestRequestTypeDef](./type_defs.md#deletethingshadowrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRetainedMessageRequestRequestTypeDef](./type_defs.md#getretainedmessagerequestrequesttypedef)
- [GetThingShadowRequestRequestTypeDef](./type_defs.md#getthingshadowrequestrequesttypedef)
- [ListNamedShadowsForThingRequestRequestTypeDef](./type_defs.md#listnamedshadowsforthingrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRetainedMessagesRequestRequestTypeDef](./type_defs.md#listretainedmessagesrequestrequesttypedef)
- [RetainedMessageSummaryTypeDef](./type_defs.md#retainedmessagesummarytypedef)
- [PublishRequestRequestTypeDef](./type_defs.md#publishrequestrequesttypedef)
- [UpdateThingShadowRequestRequestTypeDef](./type_defs.md#updatethingshadowrequestrequesttypedef)
- [DeleteThingShadowResponseTypeDef](./type_defs.md#deletethingshadowresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetRetainedMessageResponseTypeDef](./type_defs.md#getretainedmessageresponsetypedef)
- [GetThingShadowResponseTypeDef](./type_defs.md#getthingshadowresponsetypedef)
- [ListNamedShadowsForThingResponseTypeDef](./type_defs.md#listnamedshadowsforthingresponsetypedef)
- [UpdateThingShadowResponseTypeDef](./type_defs.md#updatethingshadowresponsetypedef)
- [ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef](./type_defs.md#listretainedmessagesrequestlistretainedmessagespaginatetypedef)
- [ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef)

