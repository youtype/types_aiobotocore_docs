# Examples

> [Index](../README.md) > [CodeCatalyst](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeCatalyst](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#codecatalyst)
    type annotations stubs module [types-aiobotocore-codecatalyst](https://pypi.org/project/types-aiobotocore-codecatalyst/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codecatalyst]` package installed.

Write your `CodeCatalyst` code as usual,
type checking and code completion should work out of the box.



```python
# CodeCatalystClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codecatalyst") as client:  # (1)
    result = await client.create_access_token()  # (2)
```

1. client: [CodeCatalystClient](./client.md)
2. result: [:material-code-braces: CreateAccessTokenResponseTypeDef](./type_defs.md#createaccesstokenresponsetypedef) 



```python
# ListAccessTokensPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codecatalyst") as client:  # (1)
    paginator = client.get_paginator("list_access_tokens")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeCatalystClient](./client.md)
2. paginator: [ListAccessTokensPaginator](./paginators.md#listaccesstokenspaginator)
3. item: [:material-code-braces: ListAccessTokensResponseTypeDef](./type_defs.md#listaccesstokensresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[codecatalyst]`
or a standalone `types_aiobotocore_codecatalyst` package, you have to explicitly specify
`client: CodeCatalystClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeCatalystClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.client import CodeCatalystClient
from types_aiobotocore_codecatalyst.type_defs import CreateAccessTokenResponseTypeDef
from types_aiobotocore_codecatalyst.type_defs import CreateAccessTokenRequestTypeDef


session = get_session()

async with session.create_client("codecatalyst") as client:
    client: CodeCatalystClient
    kwargs: CreateAccessTokenRequestTypeDef = {...}
    result: CreateAccessTokenResponseTypeDef = await client.create_access_token(**kwargs)
```



```python
# ListAccessTokensPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codecatalyst.client import CodeCatalystClient
from types_aiobotocore_codecatalyst.paginator import ListAccessTokensPaginator
from types_aiobotocore_codecatalyst.type_defs import ListAccessTokensResponseTypeDef


session = get_session()

async with session.create_client("codecatalyst") as client:
    client: CodeCatalystClient
    paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")
    async for item in paginator.paginate(...):
        item: ListAccessTokensResponseTypeDef
        print(item)
```


