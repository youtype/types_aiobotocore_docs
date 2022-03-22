<a id="examples-for-aiobotocore-datasync-module"></a>

# Examples for aiobotocore DataSync module

> [Index](../README.md) > [DataSync](./README.md) > Examples

- [Examples for aiobotocore DataSync module](#examples-for-aiobotocore-datasync-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[datasync]` package installed.

Write your `DataSync` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DataSyncClient
# and provides type checking and code completion
async with session.create_client("datasync") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAgentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_agents")
    async for item in paginator.paginate(...):
        # item has type ListAgentsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[datasync]` or a standalone
`types_aiobotocore_datasync` package, you have to explicitly specify
`client: DataSyncClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_datasync.client import DataSyncClient
from types_aiobotocore_datasync.type_defs import bool
from types_aiobotocore_datasync.paginator import ListAgentsPaginator

from types_aiobotocore_datasync.literals import PaginatorName



session = get_session()

async with session.create_client("datasync") as client:
    client: DataSyncClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_agents"
    paginator: ListAgentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAgentsResponseTypeDef
        print(item)
    

    
```
