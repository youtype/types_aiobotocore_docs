# Examples

> [Index](../README.md) > [AppSync](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#appsync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appsync]` package installed.

Write your `AppSync` code as usual,
type checking and code completion should work out of the box.



```python
# AppSyncClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appsync") as client:  # (1)
    result = await client.associate_api()  # (2)
```

1. client: [AppSyncClient](./client.md)
2. result: [:material-code-braces: AssociateApiResponseTypeDef](./type_defs.md#associateapiresponsetypedef) 



```python
# ListApiKeysPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appsync") as client:  # (1)
    paginator = client.get_paginator("list_api_keys")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppSyncClient](./client.md)
2. paginator: [ListApiKeysPaginator](./paginators.md#listapikeyspaginator)
3. item: [:material-code-braces: ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[appsync]`
or a standalone `types_aiobotocore_appsync` package, you have to explicitly specify
`client: AppSyncClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppSyncClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appsync.client import AppSyncClient
from types_aiobotocore_appsync.type_defs import AssociateApiResponseTypeDef
from types_aiobotocore_appsync.type_defs import AssociateApiRequestTypeDef


session = get_session()

async with session.create_client("appsync") as client:
    client: AppSyncClient
    kwargs: AssociateApiRequestTypeDef = {...}
    result: AssociateApiResponseTypeDef = await client.associate_api(**kwargs)
```



```python
# ListApiKeysPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appsync.client import AppSyncClient
from types_aiobotocore_appsync.paginator import ListApiKeysPaginator
from types_aiobotocore_appsync.type_defs import ListApiKeysResponseTypeDef


session = get_session()

async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListApiKeysPaginator = client.get_paginator("list_api_keys")
    async for item in paginator.paginate(...):
        item: ListApiKeysResponseTypeDef
        print(item)
```


