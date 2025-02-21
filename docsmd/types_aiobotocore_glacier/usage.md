# Examples

> [Index](../README.md) > [Glacier](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#glacier)
    type annotations stubs module [types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[glacier]` package installed.

Write your `Glacier` code as usual,
type checking and code completion should work out of the box.



```python
# GlacierClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("glacier") as client:  # (1)
    result = await client.abort_multipart_upload()  # (2)
```

1. client: [GlacierClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("glacier") as client:  # (1)
    paginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GlacierClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 



```python
# VaultExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("glacier") as client:  # (1)
    waiter = client.get_waiter("vault_exists")  # (2)
    await waiter.wait()
```

1. client: [GlacierClient](./client.md)
2. waiter: [VaultExistsWaiter](./waiters.md#vaultexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[glacier]`
or a standalone `types_aiobotocore_glacier` package, you have to explicitly specify
`client: GlacierClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GlacierClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_glacier.client import GlacierClient
from types_aiobotocore_glacier.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_glacier.type_defs import AbortMultipartUploadInputTypeDef


session = get_session()

async with session.create_client("glacier") as client:
    client: GlacierClient
    kwargs: AbortMultipartUploadInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.abort_multipart_upload(**kwargs)
```



```python
# ListJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_glacier.client import GlacierClient
from types_aiobotocore_glacier.paginator import ListJobsPaginator
from types_aiobotocore_glacier.type_defs import ListJobsOutputTypeDef


session = get_session()

async with session.create_client("glacier") as client:
    client: GlacierClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
    async for item in paginator.paginate(...):
        item: ListJobsOutputTypeDef
        print(item)
```



```python
# VaultExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_glacier.client import GlacierClient
from types_aiobotocore_glacier.waiter import VaultExistsWaiter


session = get_session()

async with session.create_client("glacier") as client:
    client: GlacierClient
    waiter: VaultExistsWaiter = client.get_waiter("vault_exists")
    await waiter.wait()
```
