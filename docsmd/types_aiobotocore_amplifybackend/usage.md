# Examples

> [Index](../README.md) > [AmplifyBackend](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AmplifyBackend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#amplifybackend)
    type annotations stubs module [types-aiobotocore-amplifybackend](https://pypi.org/project/types-aiobotocore-amplifybackend/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[amplifybackend]` package installed.

Write your `AmplifyBackend` code as usual,
type checking and code completion should work out of the box.



```python
# AmplifyBackendClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amplifybackend") as client:  # (1)
    result = await client.clone_backend()  # (2)
```

1. client: [AmplifyBackendClient](./client.md)
2. result: [:material-code-braces: CloneBackendResponseTypeDef](./type_defs.md#clonebackendresponsetypedef) 



```python
# ListBackendJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amplifybackend") as client:  # (1)
    paginator = client.get_paginator("list_backend_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AmplifyBackendClient](./client.md)
2. paginator: [ListBackendJobsPaginator](./paginators.md#listbackendjobspaginator)
3. item: [:material-code-braces: ListBackendJobsResponseTypeDef](./type_defs.md#listbackendjobsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[amplifybackend]`
or a standalone `types_aiobotocore_amplifybackend` package, you have to explicitly specify
`client: AmplifyBackendClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AmplifyBackendClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amplifybackend.client import AmplifyBackendClient
from types_aiobotocore_amplifybackend.type_defs import CloneBackendResponseTypeDef
from types_aiobotocore_amplifybackend.type_defs import CloneBackendRequestTypeDef


session = get_session()

async with session.create_client("amplifybackend") as client:
    client: AmplifyBackendClient
    kwargs: CloneBackendRequestTypeDef = {...}
    result: CloneBackendResponseTypeDef = await client.clone_backend(**kwargs)
```



```python
# ListBackendJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amplifybackend.client import AmplifyBackendClient
from types_aiobotocore_amplifybackend.paginator import ListBackendJobsPaginator
from types_aiobotocore_amplifybackend.type_defs import ListBackendJobsResponseTypeDef


session = get_session()

async with session.create_client("amplifybackend") as client:
    client: AmplifyBackendClient
    paginator: ListBackendJobsPaginator = client.get_paginator("list_backend_jobs")
    async for item in paginator.paginate(...):
        item: ListBackendJobsResponseTypeDef
        print(item)
```


