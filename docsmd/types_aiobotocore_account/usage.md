# Examples

> [Index](../README.md) > [Account](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#account)
    type annotations stubs module [types-aiobotocore-account](https://pypi.org/project/types-aiobotocore-account/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[account]` package installed.

Write your `Account` code as usual,
type checking and code completion should work out of the box.



```python
# AccountClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("account") as client:  # (1)
    result = await client.accept_primary_email_update()  # (2)
```

1. client: [AccountClient](./client.md)
2. result: [:material-code-braces: AcceptPrimaryEmailUpdateResponseTypeDef](./type_defs.md#acceptprimaryemailupdateresponsetypedef) 



```python
# ListRegionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("account") as client:  # (1)
    paginator = client.get_paginator("list_regions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AccountClient](./client.md)
2. paginator: [ListRegionsPaginator](./paginators.md#listregionspaginator)
3. item: [:material-code-braces: ListRegionsResponseTypeDef](./type_defs.md#listregionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[account]`
or a standalone `types_aiobotocore_account` package, you have to explicitly specify
`client: AccountClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AccountClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_account.client import AccountClient
from types_aiobotocore_account.type_defs import AcceptPrimaryEmailUpdateResponseTypeDef
from types_aiobotocore_account.type_defs import AcceptPrimaryEmailUpdateRequestTypeDef


session = get_session()

async with session.create_client("account") as client:
    client: AccountClient
    kwargs: AcceptPrimaryEmailUpdateRequestTypeDef = {...}
    result: AcceptPrimaryEmailUpdateResponseTypeDef = await client.accept_primary_email_update(**kwargs)
```



```python
# ListRegionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_account.client import AccountClient
from types_aiobotocore_account.paginator import ListRegionsPaginator
from types_aiobotocore_account.type_defs import ListRegionsResponseTypeDef


session = get_session()

async with session.create_client("account") as client:
    client: AccountClient
    paginator: ListRegionsPaginator = client.get_paginator("list_regions")
    async for item in paginator.paginate(...):
        item: ListRegionsResponseTypeDef
        print(item)
```


