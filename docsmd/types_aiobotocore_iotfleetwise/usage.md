# Examples

> [Index](../README.md) > [IoTFleetWise](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTFleetWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#iotfleetwise)
    type annotations stubs module [types-aiobotocore-iotfleetwise](https://pypi.org/project/types-aiobotocore-iotfleetwise/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotfleetwise]` package installed.

Write your `IoTFleetWise` code as usual,
type checking and code completion should work out of the box.



```python
# IoTFleetWiseClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotfleetwise") as client:  # (1)
    result = await client.batch_create_vehicle()  # (2)
```

1. client: [IoTFleetWiseClient](./client.md)
2. result: [:material-code-braces: BatchCreateVehicleResponseTypeDef](./type_defs.md#batchcreatevehicleresponsetypedef) 



```python
# GetVehicleStatusPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotfleetwise") as client:  # (1)
    paginator = client.get_paginator("get_vehicle_status")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [GetVehicleStatusPaginator](./paginators.md#getvehiclestatuspaginator)
3. item: [:material-code-braces: GetVehicleStatusResponseTypeDef](./type_defs.md#getvehiclestatusresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[iotfleetwise]`
or a standalone `types_aiobotocore_iotfleetwise` package, you have to explicitly specify
`client: IoTFleetWiseClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTFleetWiseClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.client import IoTFleetWiseClient
from types_aiobotocore_iotfleetwise.type_defs import BatchCreateVehicleResponseTypeDef
from types_aiobotocore_iotfleetwise.type_defs import BatchCreateVehicleRequestTypeDef


session = get_session()

async with session.create_client("iotfleetwise") as client:
    client: IoTFleetWiseClient
    kwargs: BatchCreateVehicleRequestTypeDef = {...}
    result: BatchCreateVehicleResponseTypeDef = await client.batch_create_vehicle(**kwargs)
```



```python
# GetVehicleStatusPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.client import IoTFleetWiseClient
from types_aiobotocore_iotfleetwise.paginator import GetVehicleStatusPaginator
from types_aiobotocore_iotfleetwise.type_defs import GetVehicleStatusResponseTypeDef


session = get_session()

async with session.create_client("iotfleetwise") as client:
    client: IoTFleetWiseClient
    paginator: GetVehicleStatusPaginator = client.get_paginator("get_vehicle_status")
    async for item in paginator.paginate(...):
        item: GetVehicleStatusResponseTypeDef
        print(item)
```


