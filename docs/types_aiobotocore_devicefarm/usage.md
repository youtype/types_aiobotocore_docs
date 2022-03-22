<a id="examples-for-aiobotocore-devicefarm-module"></a>

# Examples for aiobotocore DeviceFarm module

> [Index](../README.md) > [DeviceFarm](./README.md) > Examples

- [Examples for aiobotocore DeviceFarm module](#examples-for-aiobotocore-devicefarm-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[devicefarm]` package installed.

Write your `DeviceFarm` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DeviceFarmClient
# and provides type checking and code completion
async with session.create_client("devicefarm") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetOfferingStatusPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_offering_status")
    async for item in paginator.paginate(...):
        # item has type GetOfferingStatusResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[devicefarm]` or a standalone
`types_aiobotocore_devicefarm` package, you have to explicitly specify
`client: DeviceFarmClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_devicefarm.client import DeviceFarmClient
from types_aiobotocore_devicefarm.type_defs import bool
from types_aiobotocore_devicefarm.paginator import GetOfferingStatusPaginator

from types_aiobotocore_devicefarm.literals import PaginatorName



session = get_session()

async with session.create_client("devicefarm") as client:
    client: DeviceFarmClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_offering_status"
    paginator: GetOfferingStatusPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetOfferingStatusResultTypeDef
        print(item)
    

    
```
