<a id="examples-for-aiobotocore-iotfleethub-module"></a>

# Examples for aiobotocore IoTFleetHub module

> [Index](../README.md) > [IoTFleetHub](./README.md) > Examples

- [Examples for aiobotocore IoTFleetHub module](#examples-for-aiobotocore-iotfleethub-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotfleethub]` package installed.

Write your `IoTFleetHub` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTFleetHubClient
# and provides type checking and code completion
async with session.create_client("iotfleethub") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListApplicationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        # item has type ListApplicationsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotfleethub]` or a standalone
`types_aiobotocore_iotfleethub` package, you have to explicitly specify
`client: IoTFleetHubClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotfleethub.client import IoTFleetHubClient
from types_aiobotocore_iotfleethub.type_defs import bool
from types_aiobotocore_iotfleethub.paginator import ListApplicationsPaginator

from types_aiobotocore_iotfleethub.literals import PaginatorName



session = get_session()

async with session.create_client("iotfleethub") as client:
    client: IoTFleetHubClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_applications"
    paginator: ListApplicationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)
    

    
```
