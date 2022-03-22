<a id="examples-for-aiobotocore-groundstation-module"></a>

# Examples for aiobotocore GroundStation module

> [Index](../README.md) > [GroundStation](./README.md) > Examples

- [Examples for aiobotocore GroundStation module](#examples-for-aiobotocore-groundstation-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[groundstation]` package installed.

Write your `GroundStation` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GroundStationClient
# and provides type checking and code completion
async with session.create_client("groundstation") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListConfigsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_configs")
    async for item in paginator.paginate(...):
        # item has type ListConfigsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[groundstation]` or a standalone
`types_aiobotocore_groundstation` package, you have to explicitly specify
`client: GroundStationClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_groundstation.client import GroundStationClient
from types_aiobotocore_groundstation.type_defs import bool
from types_aiobotocore_groundstation.paginator import ListConfigsPaginator

from types_aiobotocore_groundstation.literals import PaginatorName



session = get_session()

async with session.create_client("groundstation") as client:
    client: GroundStationClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_configs"
    paginator: ListConfigsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListConfigsResponseTypeDef
        print(item)
    

    
```
