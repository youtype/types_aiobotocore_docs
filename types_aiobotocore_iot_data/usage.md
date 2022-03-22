<a id="examples-for-aiobotocore-iotdataplane-module"></a>

# Examples for aiobotocore IoTDataPlane module

> [Index](../README.md) > [IoTDataPlane](./README.md) > Examples

- [Examples for aiobotocore IoTDataPlane module](#examples-for-aiobotocore-iotdataplane-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iot-data]` package installed.

Write your `IoTDataPlane` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTDataPlaneClient
# and provides type checking and code completion
async with session.create_client("iot-data") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListRetainedMessagesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_retained_messages")
    async for item in paginator.paginate(...):
        # item has type ListRetainedMessagesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iot-data]` or a standalone
`types_aiobotocore_iot_data` package, you have to explicitly specify
`client: IoTDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot_data.client import IoTDataPlaneClient
from types_aiobotocore_iot_data.type_defs import bool
from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator

from types_aiobotocore_iot_data.literals import PaginatorName



session = get_session()

async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_retained_messages"
    paginator: ListRetainedMessagesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListRetainedMessagesResponseTypeDef
        print(item)
    

    
```
