# Examples

> [Index](../README.md) > [IoTDataPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#iotdataplane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iot-data]` package installed.

Write your `IoTDataPlane` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# IoTDataPlaneClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-data") as client:  # (1)
    result = await client.delete_connection()  # (2)
```

1. client: [IoTDataPlaneClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)



#### Paginator usage example

```python
# ListRetainedMessagesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-data") as client:  # (1)
    paginator = client.get_paginator("list_retained_messages")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTDataPlaneClient](./client.md)
2. paginator: [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)
3. item: [:material-code-braces: ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[iot-data]`
or a standalone `types_aiobotocore_iot_data` package, you have to explicitly specify
`client: IoTDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# IoTDataPlaneClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_data.client import IoTDataPlaneClient
from types_aiobotocore_iot_data.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_iot_data.type_defs import DeleteConnectionRequestTypeDef


session = get_session()

async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient
    kwargs: DeleteConnectionRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.delete_connection(**kwargs)
```



#### Paginator usage example

```python
# ListRetainedMessagesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_data.client import IoTDataPlaneClient
from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator
from types_aiobotocore_iot_data.type_defs import ListRetainedMessagesResponseTypeDef


session = get_session()

async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient
    paginator: ListRetainedMessagesPaginator = client.get_paginator("list_retained_messages")
    async for item in paginator.paginate(...):
        item: ListRetainedMessagesResponseTypeDef
        print(item)
```


