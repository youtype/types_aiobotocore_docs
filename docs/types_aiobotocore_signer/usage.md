<a id="examples-for-aiobotocore-signer-module"></a>

# Examples for aiobotocore signer module

> [Index](../README.md) > [signer](./README.md) > Examples

- [Examples for aiobotocore signer module](#examples-for-aiobotocore-signer-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[signer]` package installed.

Write your `signer` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type signerClient
# and provides type checking and code completion
async with session.create_client("signer") as client:
    
    # result has type AddProfilePermissionResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_profile_permission()
    

    
    # paginator has type ListSigningJobsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_signing_jobs")
    async for item in paginator.paginate(...):
        # item has type ListSigningJobsResponseTypeDef
        print(item)
    

    
    # waiter has type SuccessfulSigningJobWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("successful_signing_job")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[signer]` or a standalone
`types_aiobotocore_signer` package, you have to explicitly specify
`client: signerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_signer.client import signerClient
from types_aiobotocore_signer.type_defs import AddProfilePermissionResponseTypeDef
from types_aiobotocore_signer.paginator import ListSigningJobsPaginator
from types_aiobotocore_signer.waiter import SuccessfulSigningJobWaiter
from types_aiobotocore_signer.literals import PaginatorName
from types_aiobotocore_signer.literals import WaiterName


session = get_session()

async with session.create_client("signer") as client:
    client: signerClient

    
    result: AddProfilePermissionResponseTypeDef = client.add_profile_permission()
    

    
    paginator_name: PaginatorName = "list_signing_jobs"
    paginator: ListSigningJobsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListSigningJobsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "successful_signing_job"
    waiter: SuccessfulSigningJobWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
