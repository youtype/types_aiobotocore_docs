<a id="examples-for-aiobotocore-braket-module"></a>

# Examples for aiobotocore Braket module

> [Index](../README.md) > [Braket](./README.md) > Examples

- [Examples for aiobotocore Braket module](#examples-for-aiobotocore-braket-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[braket]` package installed.

Write your `Braket` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type BraketClient
# and provides type checking and code completion
async with session.create_client("braket") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type SearchDevicesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("search_devices")
    async for item in paginator.paginate(...):
        # item has type SearchDevicesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[braket]` or a standalone
`types_aiobotocore_braket` package, you have to explicitly specify
`client: BraketClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_braket.client import BraketClient
from types_aiobotocore_braket.type_defs import bool
from types_aiobotocore_braket.paginator import SearchDevicesPaginator

from types_aiobotocore_braket.literals import PaginatorName



session = get_session()

async with session.create_client("braket") as client:
    client: BraketClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "search_devices"
    paginator: SearchDevicesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: SearchDevicesResponseTypeDef
        print(item)
    

    
```
