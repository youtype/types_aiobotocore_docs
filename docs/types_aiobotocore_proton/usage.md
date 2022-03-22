<a id="examples-for-aiobotocore-proton-module"></a>

# Examples for aiobotocore Proton module

> [Index](../README.md) > [Proton](./README.md) > Examples

- [Examples for aiobotocore Proton module](#examples-for-aiobotocore-proton-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[proton]` package installed.

Write your `Proton` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ProtonClient
# and provides type checking and code completion
async with session.create_client("proton") as client:
    
    # result has type AcceptEnvironmentAccountConnectionOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_environment_account_connection()
    

    
    # paginator has type ListEnvironmentAccountConnectionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_environment_account_connections")
    async for item in paginator.paginate(...):
        # item has type ListEnvironmentAccountConnectionsOutputTypeDef
        print(item)
    

    
    # waiter has type EnvironmentDeployedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("environment_deployed")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[proton]` or a standalone
`types_aiobotocore_proton` package, you have to explicitly specify
`client: ProtonClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_proton.client import ProtonClient
from types_aiobotocore_proton.type_defs import AcceptEnvironmentAccountConnectionOutputTypeDef
from types_aiobotocore_proton.paginator import ListEnvironmentAccountConnectionsPaginator
from types_aiobotocore_proton.waiter import EnvironmentDeployedWaiter
from types_aiobotocore_proton.literals import PaginatorName
from types_aiobotocore_proton.literals import WaiterName


session = get_session()

async with session.create_client("proton") as client:
    client: ProtonClient

    
    result: AcceptEnvironmentAccountConnectionOutputTypeDef = client.accept_environment_account_connection()
    

    
    paginator_name: PaginatorName = "list_environment_account_connections"
    paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListEnvironmentAccountConnectionsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "environment_deployed"
    waiter: EnvironmentDeployedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
