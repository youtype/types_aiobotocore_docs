# Examples

> [Index](../README.md) > [Signer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[signer]` package installed.

Write your `Signer` code as usual,
type checking and code completion should work out of the box.



```python
# SignerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("signer") as client:  # (1)
    result = await client.add_profile_permission()  # (2)
```

1. client: [SignerClient](./client.md)
2. result: [:material-code-braces: AddProfilePermissionResponseTypeDef](./type_defs.md#addprofilepermissionresponsetypedef) 



```python
# ListSigningJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("signer") as client:  # (1)
    paginator = client.get_paginator("list_signing_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SignerClient](./client.md)
2. paginator: [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
3. item: [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 



```python
# SuccessfulSigningJobWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("signer") as client:  # (1)
    waiter = client.get_waiter("successful_signing_job")  # (2)
    await waiter.wait()
```

1. client: [SignerClient](./client.md)
2. waiter: [SuccessfulSigningJobWaiter](./waiters.md#successfulsigningjobwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[signer]`
or a standalone `types_aiobotocore_signer` package, you have to explicitly specify
`client: SignerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SignerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_signer.client import SignerClient
from types_aiobotocore_signer.type_defs import AddProfilePermissionResponseTypeDef
from types_aiobotocore_signer.type_defs import AddProfilePermissionRequestTypeDef


session = get_session()

async with session.create_client("signer") as client:
    client: SignerClient
    kwargs: AddProfilePermissionRequestTypeDef = {...}
    result: AddProfilePermissionResponseTypeDef = await client.add_profile_permission(**kwargs)
```



```python
# ListSigningJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_signer.client import SignerClient
from types_aiobotocore_signer.paginator import ListSigningJobsPaginator
from types_aiobotocore_signer.type_defs import ListSigningJobsResponseTypeDef


session = get_session()

async with session.create_client("signer") as client:
    client: SignerClient
    paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
    async for item in paginator.paginate(...):
        item: ListSigningJobsResponseTypeDef
        print(item)
```



```python
# SuccessfulSigningJobWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_signer.client import SignerClient
from types_aiobotocore_signer.waiter import SuccessfulSigningJobWaiter


session = get_session()

async with session.create_client("signer") as client:
    client: SignerClient
    waiter: SuccessfulSigningJobWaiter = client.get_waiter("successful_signing_job")
    await waiter.wait()
```
