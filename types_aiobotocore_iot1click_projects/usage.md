<a id="examples-for-aiobotocore-iot1clickprojects-module"></a>

# Examples for aiobotocore IoT1ClickProjects module

> [Index](../README.md) > [IoT1ClickProjects](./README.md) > Examples

- [Examples for aiobotocore IoT1ClickProjects module](#examples-for-aiobotocore-iot1clickprojects-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iot1click-projects]` package installed.

Write your `IoT1ClickProjects` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoT1ClickProjectsClient
# and provides type checking and code completion
async with session.create_client("iot1click-projects") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_device_with_placement()
    

    
    # paginator has type ListPlacementsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_placements")
    async for item in paginator.paginate(...):
        # item has type ListPlacementsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iot1click-projects]` or a standalone
`types_aiobotocore_iot1click_projects` package, you have to explicitly specify
`client: IoT1ClickProjectsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_projects.client import IoT1ClickProjectsClient
from types_aiobotocore_iot1click_projects.type_defs import Dict[str, Any]
from types_aiobotocore_iot1click_projects.paginator import ListPlacementsPaginator

from types_aiobotocore_iot1click_projects.literals import PaginatorName



session = get_session()

async with session.create_client("iot1click-projects") as client:
    client: IoT1ClickProjectsClient

    
    result: Dict[str, Any] = client.associate_device_with_placement()
    

    
    paginator_name: PaginatorName = "list_placements"
    paginator: ListPlacementsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListPlacementsResponseTypeDef
        print(item)
    

    
```
