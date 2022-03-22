<a id="examples-for-aiobotocore-appsync-module"></a>

# Examples for aiobotocore AppSync module

> [Index](../README.md) > [AppSync](./README.md) > Examples

- [Examples for aiobotocore AppSync module](#examples-for-aiobotocore-appsync-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[appsync]` package installed.

Write your `AppSync` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AppSyncClient
# and provides type checking and code completion
async with session.create_client("appsync") as client:
    
    # result has type AssociateApiResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_api()
    

    
    # paginator has type ListApiKeysPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_api_keys")
    async for item in paginator.paginate(...):
        # item has type ListApiKeysResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[appsync]` or a standalone
`types_aiobotocore_appsync` package, you have to explicitly specify
`client: AppSyncClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_appsync.client import AppSyncClient
from types_aiobotocore_appsync.type_defs import AssociateApiResponseTypeDef
from types_aiobotocore_appsync.paginator import ListApiKeysPaginator

from types_aiobotocore_appsync.literals import PaginatorName



session = get_session()

async with session.create_client("appsync") as client:
    client: AppSyncClient

    
    result: AssociateApiResponseTypeDef = client.associate_api()
    

    
    paginator_name: PaginatorName = "list_api_keys"
    paginator: ListApiKeysPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListApiKeysResponseTypeDef
        print(item)
    

    
```
