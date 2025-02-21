# Examples

> [Index](../README.md) > [B2BI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#b2bi)
    type annotations stubs module [types-aiobotocore-b2bi](https://pypi.org/project/types-aiobotocore-b2bi/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[b2bi]` package installed.

Write your `B2BI` code as usual,
type checking and code completion should work out of the box.



```python
# B2BIClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("b2bi") as client:  # (1)
    result = await client.create_capability()  # (2)
```

1. client: [B2BIClient](./client.md)
2. result: [:material-code-braces: CreateCapabilityResponseTypeDef](./type_defs.md#createcapabilityresponsetypedef) 



```python
# ListCapabilitiesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("b2bi") as client:  # (1)
    paginator = client.get_paginator("list_capabilities")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [B2BIClient](./client.md)
2. paginator: [ListCapabilitiesPaginator](./paginators.md#listcapabilitiespaginator)
3. item: [:material-code-braces: ListCapabilitiesResponseTypeDef](./type_defs.md#listcapabilitiesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[b2bi]`
or a standalone `types_aiobotocore_b2bi` package, you have to explicitly specify
`client: B2BIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# B2BIClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_b2bi.client import B2BIClient
from types_aiobotocore_b2bi.type_defs import CreateCapabilityResponseTypeDef
from types_aiobotocore_b2bi.type_defs import CreateCapabilityRequestTypeDef


session = get_session()

async with session.create_client("b2bi") as client:
    client: B2BIClient
    kwargs: CreateCapabilityRequestTypeDef = {...}
    result: CreateCapabilityResponseTypeDef = await client.create_capability(**kwargs)
```



```python
# ListCapabilitiesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_b2bi.client import B2BIClient
from types_aiobotocore_b2bi.paginator import ListCapabilitiesPaginator
from types_aiobotocore_b2bi.type_defs import ListCapabilitiesResponseTypeDef


session = get_session()

async with session.create_client("b2bi") as client:
    client: B2BIClient
    paginator: ListCapabilitiesPaginator = client.get_paginator("list_capabilities")
    async for item in paginator.paginate(...):
        item: ListCapabilitiesResponseTypeDef
        print(item)
```


