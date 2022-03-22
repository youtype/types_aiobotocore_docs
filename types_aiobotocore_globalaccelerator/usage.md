<a id="examples-for-aiobotocore-globalaccelerator-module"></a>

# Examples for aiobotocore GlobalAccelerator module

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Examples

- [Examples for aiobotocore GlobalAccelerator module](#examples-for-aiobotocore-globalaccelerator-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[globalaccelerator]` package installed.

Write your `GlobalAccelerator` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GlobalAcceleratorClient
# and provides type checking and code completion
async with session.create_client("globalaccelerator") as client:
    
    # result has type AddCustomRoutingEndpointsResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_custom_routing_endpoints()
    

    
    # paginator has type ListAcceleratorsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_accelerators")
    async for item in paginator.paginate(...):
        # item has type ListAcceleratorsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[globalaccelerator]` or a standalone
`types_aiobotocore_globalaccelerator` package, you have to explicitly specify
`client: GlobalAcceleratorClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.client import GlobalAcceleratorClient
from types_aiobotocore_globalaccelerator.type_defs import AddCustomRoutingEndpointsResponseTypeDef
from types_aiobotocore_globalaccelerator.paginator import ListAcceleratorsPaginator

from types_aiobotocore_globalaccelerator.literals import PaginatorName



session = get_session()

async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient

    
    result: AddCustomRoutingEndpointsResponseTypeDef = client.add_custom_routing_endpoints()
    

    
    paginator_name: PaginatorName = "list_accelerators"
    paginator: ListAcceleratorsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAcceleratorsResponseTypeDef
        print(item)
    

    
```
