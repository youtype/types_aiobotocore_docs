<a id="examples-for-aiobotocore-glacier-module"></a>

# Examples for aiobotocore Glacier module

> [Index](../README.md) > [Glacier](./README.md) > Examples

- [Examples for aiobotocore Glacier module](#examples-for-aiobotocore-glacier-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[glacier]` package installed.

Write your `Glacier` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GlacierClient
# and provides type checking and code completion
async with session.create_client("glacier") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.abort_multipart_upload()
    

    
    # paginator has type ListJobsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_jobs")
    async for item in paginator.paginate(...):
        # item has type ListJobsOutputTypeDef
        print(item)
    

    
    # waiter has type VaultExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("vault_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[glacier]` or a standalone
`types_aiobotocore_glacier` package, you have to explicitly specify
`client: GlacierClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_glacier.client import GlacierClient
from types_aiobotocore_glacier.type_defs import None
from types_aiobotocore_glacier.paginator import ListJobsPaginator
from types_aiobotocore_glacier.waiter import VaultExistsWaiter
from types_aiobotocore_glacier.literals import PaginatorName
from types_aiobotocore_glacier.literals import WaiterName


session = get_session()

async with session.create_client("glacier") as client:
    client: GlacierClient

    
    result: None = client.abort_multipart_upload()
    

    
    paginator_name: PaginatorName = "list_jobs"
    paginator: ListJobsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListJobsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "vault_exists"
    waiter: VaultExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
