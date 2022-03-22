<a id="examples-for-aiobotocore-nimblestudio-module"></a>

# Examples for aiobotocore NimbleStudio module

> [Index](../README.md) > [NimbleStudio](./README.md) > Examples

- [Examples for aiobotocore NimbleStudio module](#examples-for-aiobotocore-nimblestudio-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[nimble]` package installed.

Write your `NimbleStudio` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type NimbleStudioClient
# and provides type checking and code completion
async with session.create_client("nimble") as client:
    
    # result has type AcceptEulasResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_eulas()
    

    
    # paginator has type ListEulaAcceptancesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_eula_acceptances")
    async for item in paginator.paginate(...):
        # item has type ListEulaAcceptancesResponseTypeDef
        print(item)
    

    
    # waiter has type LaunchProfileDeletedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("launch_profile_deleted")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[nimble]` or a standalone
`types_aiobotocore_nimble` package, you have to explicitly specify
`client: NimbleStudioClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_nimble.client import NimbleStudioClient
from types_aiobotocore_nimble.type_defs import AcceptEulasResponseTypeDef
from types_aiobotocore_nimble.paginator import ListEulaAcceptancesPaginator
from types_aiobotocore_nimble.waiter import LaunchProfileDeletedWaiter
from types_aiobotocore_nimble.literals import PaginatorName
from types_aiobotocore_nimble.literals import WaiterName


session = get_session()

async with session.create_client("nimble") as client:
    client: NimbleStudioClient

    
    result: AcceptEulasResponseTypeDef = client.accept_eulas()
    

    
    paginator_name: PaginatorName = "list_eula_acceptances"
    paginator: ListEulaAcceptancesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListEulaAcceptancesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "launch_profile_deleted"
    waiter: LaunchProfileDeletedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
