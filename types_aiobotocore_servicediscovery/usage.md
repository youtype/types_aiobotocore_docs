<a id="examples-for-aiobotocore-servicediscovery-module"></a>

# Examples for aiobotocore ServiceDiscovery module

> [Index](../README.md) > [ServiceDiscovery](./README.md) > Examples

- [Examples for aiobotocore ServiceDiscovery module](#examples-for-aiobotocore-servicediscovery-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[servicediscovery]` package installed.

Write your `ServiceDiscovery` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ServiceDiscoveryClient
# and provides type checking and code completion
async with session.create_client("servicediscovery") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListInstancesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_instances")
    async for item in paginator.paginate(...):
        # item has type ListInstancesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[servicediscovery]` or a standalone
`types_aiobotocore_servicediscovery` package, you have to explicitly specify
`client: ServiceDiscoveryClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_servicediscovery.client import ServiceDiscoveryClient
from types_aiobotocore_servicediscovery.type_defs import bool
from types_aiobotocore_servicediscovery.paginator import ListInstancesPaginator

from types_aiobotocore_servicediscovery.literals import PaginatorName



session = get_session()

async with session.create_client("servicediscovery") as client:
    client: ServiceDiscoveryClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_instances"
    paginator: ListInstancesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListInstancesResponseTypeDef
        print(item)
    

    
```
