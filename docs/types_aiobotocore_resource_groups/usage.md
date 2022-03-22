<a id="examples-for-aiobotocore-resourcegroups-module"></a>

# Examples for aiobotocore ResourceGroups module

> [Index](../README.md) > [ResourceGroups](./README.md) > Examples

- [Examples for aiobotocore ResourceGroups module](#examples-for-aiobotocore-resourcegroups-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[resource-groups]` package installed.

Write your `ResourceGroups` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ResourceGroupsClient
# and provides type checking and code completion
async with session.create_client("resource-groups") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListGroupResourcesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_group_resources")
    async for item in paginator.paginate(...):
        # item has type ListGroupResourcesOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[resource-groups]` or a standalone
`types_aiobotocore_resource_groups` package, you have to explicitly specify
`client: ResourceGroupsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.client import ResourceGroupsClient
from types_aiobotocore_resource_groups.type_defs import bool
from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator

from types_aiobotocore_resource_groups.literals import PaginatorName



session = get_session()

async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_group_resources"
    paginator: ListGroupResourcesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListGroupResourcesOutputTypeDef
        print(item)
    

    
```
