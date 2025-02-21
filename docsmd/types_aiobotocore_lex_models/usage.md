# Examples

> [Index](../README.md) > [LexModelBuildingService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LexModelBuildingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#lexmodelbuildingservice)
    type annotations stubs module [types-aiobotocore-lex-models](https://pypi.org/project/types-aiobotocore-lex-models/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[lex-models]` package installed.

Write your `LexModelBuildingService` code as usual,
type checking and code completion should work out of the box.



```python
# LexModelBuildingServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lex-models") as client:  # (1)
    result = await client.create_bot_version()  # (2)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. result: [:material-code-braces: CreateBotVersionResponseTypeDef](./type_defs.md#createbotversionresponsetypedef) 



```python
# GetBotAliasesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lex-models") as client:  # (1)
    paginator = client.get_paginator("get_bot_aliases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LexModelBuildingServiceClient](./client.md)
2. paginator: [GetBotAliasesPaginator](./paginators.md#getbotaliasespaginator)
3. item: [:material-code-braces: GetBotAliasesResponseTypeDef](./type_defs.md#getbotaliasesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[lex-models]`
or a standalone `types_aiobotocore_lex_models` package, you have to explicitly specify
`client: LexModelBuildingServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LexModelBuildingServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lex_models.client import LexModelBuildingServiceClient
from types_aiobotocore_lex_models.type_defs import CreateBotVersionResponseTypeDef
from types_aiobotocore_lex_models.type_defs import CreateBotVersionRequestTypeDef


session = get_session()

async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    kwargs: CreateBotVersionRequestTypeDef = {...}
    result: CreateBotVersionResponseTypeDef = await client.create_bot_version(**kwargs)
```



```python
# GetBotAliasesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lex_models.client import LexModelBuildingServiceClient
from types_aiobotocore_lex_models.paginator import GetBotAliasesPaginator
from types_aiobotocore_lex_models.type_defs import GetBotAliasesResponseTypeDef


session = get_session()

async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetBotAliasesPaginator = client.get_paginator("get_bot_aliases")
    async for item in paginator.paginate(...):
        item: GetBotAliasesResponseTypeDef
        print(item)
```


