# Examples

> [Index](../README.md) > [FreeTier](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier)
    type annotations stubs module [types-aiobotocore-freetier](https://pypi.org/project/types-aiobotocore-freetier/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[freetier]` package installed.

Write your `FreeTier` code as usual,
type checking and code completion should work out of the box.



```python
# FreeTierClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("freetier") as client:  # (1)
    result = await client.get_free_tier_usage()  # (2)
```

1. client: [FreeTierClient](./client.md)
2. result: [:material-code-braces: GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef) 



```python
# GetFreeTierUsagePaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("freetier") as client:  # (1)
    paginator = client.get_paginator("get_free_tier_usage")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FreeTierClient](./client.md)
2. paginator: [GetFreeTierUsagePaginator](./paginators.md#getfreetierusagepaginator)
3. item: [:material-code-braces: GetFreeTierUsageResponseTypeDef](./type_defs.md#getfreetierusageresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[freetier]`
or a standalone `types_aiobotocore_freetier` package, you have to explicitly specify
`client: FreeTierClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# FreeTierClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_freetier.client import FreeTierClient
from types_aiobotocore_freetier.type_defs import GetFreeTierUsageResponseTypeDef
from types_aiobotocore_freetier.type_defs import GetFreeTierUsageRequestTypeDef


session = get_session()

async with session.create_client("freetier") as client:
    client: FreeTierClient
    kwargs: GetFreeTierUsageRequestTypeDef = {...}
    result: GetFreeTierUsageResponseTypeDef = await client.get_free_tier_usage(**kwargs)
```



```python
# GetFreeTierUsagePaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_freetier.client import FreeTierClient
from types_aiobotocore_freetier.paginator import GetFreeTierUsagePaginator
from types_aiobotocore_freetier.type_defs import GetFreeTierUsageResponseTypeDef


session = get_session()

async with session.create_client("freetier") as client:
    client: FreeTierClient
    paginator: GetFreeTierUsagePaginator = client.get_paginator("get_free_tier_usage")
    async for item in paginator.paginate(...):
        item: GetFreeTierUsageResponseTypeDef
        print(item)
```


