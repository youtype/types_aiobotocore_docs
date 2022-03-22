<a id="examples-for-aiobotocore-locationservice-module"></a>

# Examples for aiobotocore LocationService module

> [Index](../README.md) > [LocationService](./README.md) > Examples

- [Examples for aiobotocore LocationService module](#examples-for-aiobotocore-locationservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[location]` package installed.

Write your `LocationService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LocationServiceClient
# and provides type checking and code completion
async with session.create_client("location") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_tracker_consumer()
    

    
    # paginator has type GetDevicePositionHistoryPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_device_position_history")
    async for item in paginator.paginate(...):
        # item has type GetDevicePositionHistoryResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[location]` or a standalone
`types_aiobotocore_location` package, you have to explicitly specify
`client: LocationServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_location.client import LocationServiceClient
from types_aiobotocore_location.type_defs import Dict[str, Any]
from types_aiobotocore_location.paginator import GetDevicePositionHistoryPaginator

from types_aiobotocore_location.literals import PaginatorName



session = get_session()

async with session.create_client("location") as client:
    client: LocationServiceClient

    
    result: Dict[str, Any] = client.associate_tracker_consumer()
    

    
    paginator_name: PaginatorName = "get_device_position_history"
    paginator: GetDevicePositionHistoryPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetDevicePositionHistoryResponseTypeDef
        print(item)
    

    
```
