<a id="examples-for-aiobotocore-codestarnotifications-module"></a>

# Examples for aiobotocore CodeStarNotifications module

> [Index](../README.md) > [CodeStarNotifications](./README.md) > Examples

- [Examples for aiobotocore CodeStarNotifications module](#examples-for-aiobotocore-codestarnotifications-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codestar-notifications]` package installed.

Write your `CodeStarNotifications` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeStarNotificationsClient
# and provides type checking and code completion
async with session.create_client("codestar-notifications") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListEventTypesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_event_types")
    async for item in paginator.paginate(...):
        # item has type ListEventTypesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codestar-notifications]` or a standalone
`types_aiobotocore_codestar_notifications` package, you have to explicitly
specify `client: CodeStarNotificationsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar_notifications.client import CodeStarNotificationsClient
from types_aiobotocore_codestar_notifications.type_defs import bool
from types_aiobotocore_codestar_notifications.paginator import ListEventTypesPaginator

from types_aiobotocore_codestar_notifications.literals import PaginatorName



session = get_session()

async with session.create_client("codestar-notifications") as client:
    client: CodeStarNotificationsClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_event_types"
    paginator: ListEventTypesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListEventTypesResultTypeDef
        print(item)
    

    
```
