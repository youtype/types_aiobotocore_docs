<a id="examples-for-aiobotocore-lightsail-module"></a>

# Examples for aiobotocore Lightsail module

> [Index](../README.md) > [Lightsail](./README.md) > Examples

- [Examples for aiobotocore Lightsail module](#examples-for-aiobotocore-lightsail-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lightsail]` package installed.

Write your `Lightsail` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LightsailClient
# and provides type checking and code completion
async with session.create_client("lightsail") as client:
    
    # result has type AllocateStaticIpResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.allocate_static_ip()
    

    
    # paginator has type GetActiveNamesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_active_names")
    async for item in paginator.paginate(...):
        # item has type GetActiveNamesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lightsail]` or a standalone
`types_aiobotocore_lightsail` package, you have to explicitly specify
`client: LightsailClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lightsail.client import LightsailClient
from types_aiobotocore_lightsail.type_defs import AllocateStaticIpResultTypeDef
from types_aiobotocore_lightsail.paginator import GetActiveNamesPaginator

from types_aiobotocore_lightsail.literals import PaginatorName



session = get_session()

async with session.create_client("lightsail") as client:
    client: LightsailClient

    
    result: AllocateStaticIpResultTypeDef = client.allocate_static_ip()
    

    
    paginator_name: PaginatorName = "get_active_names"
    paginator: GetActiveNamesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetActiveNamesResultTypeDef
        print(item)
    

    
```
