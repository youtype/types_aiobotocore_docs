<a id="examples-for-aiobotocore-ecs-module"></a>

# Examples for aiobotocore ECS module

> [Index](../README.md) > [ECS](./README.md) > Examples

- [Examples for aiobotocore ECS module](#examples-for-aiobotocore-ecs-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ecs]` package installed.

Write your `ECS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ECSClient
# and provides type checking and code completion
async with session.create_client("ecs") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAccountSettingsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_account_settings")
    async for item in paginator.paginate(...):
        # item has type ListAccountSettingsResponseTypeDef
        print(item)
    

    
    # waiter has type ServicesInactiveWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("services_inactive")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ecs]` or a standalone `types_aiobotocore_ecs`
package, you have to explicitly specify `client: ECSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecs.client import ECSClient
from types_aiobotocore_ecs.type_defs import bool
from types_aiobotocore_ecs.paginator import ListAccountSettingsPaginator
from types_aiobotocore_ecs.waiter import ServicesInactiveWaiter
from types_aiobotocore_ecs.literals import PaginatorName
from types_aiobotocore_ecs.literals import WaiterName


session = get_session()

async with session.create_client("ecs") as client:
    client: ECSClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_account_settings"
    paginator: ListAccountSettingsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccountSettingsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "services_inactive"
    waiter: ServicesInactiveWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
