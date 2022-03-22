<a id="examples-for-aiobotocore-transfer-module"></a>

# Examples for aiobotocore Transfer module

> [Index](../README.md) > [Transfer](./README.md) > Examples

- [Examples for aiobotocore Transfer module](#examples-for-aiobotocore-transfer-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[transfer]` package installed.

Write your `Transfer` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type TransferClient
# and provides type checking and code completion
async with session.create_client("transfer") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAccessesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_accesses")
    async for item in paginator.paginate(...):
        # item has type ListAccessesResponseTypeDef
        print(item)
    

    
    # waiter has type ServerOfflineWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("server_offline")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[transfer]` or a standalone
`types_aiobotocore_transfer` package, you have to explicitly specify
`client: TransferClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.client import TransferClient
from types_aiobotocore_transfer.type_defs import bool
from types_aiobotocore_transfer.paginator import ListAccessesPaginator
from types_aiobotocore_transfer.waiter import ServerOfflineWaiter
from types_aiobotocore_transfer.literals import PaginatorName
from types_aiobotocore_transfer.literals import WaiterName


session = get_session()

async with session.create_client("transfer") as client:
    client: TransferClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_accesses"
    paginator: ListAccessesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccessesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "server_offline"
    waiter: ServerOfflineWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
