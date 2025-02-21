# Examples

> [Index](../README.md) > [Shield](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Shield](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#shield)
    type annotations stubs module [types-aiobotocore-shield](https://pypi.org/project/types-aiobotocore-shield/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[shield]` package installed.

Write your `Shield` code as usual,
type checking and code completion should work out of the box.



```python
# ShieldClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("shield") as client:  # (1)
    result = await client.create_protection()  # (2)
```

1. client: [ShieldClient](./client.md)
2. result: [:material-code-braces: CreateProtectionResponseTypeDef](./type_defs.md#createprotectionresponsetypedef) 



```python
# ListAttacksPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("shield") as client:  # (1)
    paginator = client.get_paginator("list_attacks")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ShieldClient](./client.md)
2. paginator: [ListAttacksPaginator](./paginators.md#listattackspaginator)
3. item: [:material-code-braces: ListAttacksResponseTypeDef](./type_defs.md#listattacksresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[shield]`
or a standalone `types_aiobotocore_shield` package, you have to explicitly specify
`client: ShieldClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ShieldClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_shield.client import ShieldClient
from types_aiobotocore_shield.type_defs import CreateProtectionResponseTypeDef
from types_aiobotocore_shield.type_defs import CreateProtectionRequestTypeDef


session = get_session()

async with session.create_client("shield") as client:
    client: ShieldClient
    kwargs: CreateProtectionRequestTypeDef = {...}
    result: CreateProtectionResponseTypeDef = await client.create_protection(**kwargs)
```



```python
# ListAttacksPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_shield.client import ShieldClient
from types_aiobotocore_shield.paginator import ListAttacksPaginator
from types_aiobotocore_shield.type_defs import ListAttacksResponseTypeDef


session = get_session()

async with session.create_client("shield") as client:
    client: ShieldClient
    paginator: ListAttacksPaginator = client.get_paginator("list_attacks")
    async for item in paginator.paginate(...):
        item: ListAttacksResponseTypeDef
        print(item)
```


