# Examples

> [Index](../README.md) > [Outposts](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[outposts]` package installed.

Write your `Outposts` code as usual,
type checking and code completion should work out of the box.



```python
# OutpostsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("outposts") as client:  # (1)
    result = await client.create_order()  # (2)
```

1. client: [OutpostsClient](./client.md)
2. result: [:material-code-braces: CreateOrderOutputTypeDef](./type_defs.md#createorderoutputtypedef) 



```python
# GetOutpostInstanceTypesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("outposts") as client:  # (1)
    paginator = client.get_paginator("get_outpost_instance_types")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [GetOutpostInstanceTypesPaginator](./paginators.md#getoutpostinstancetypespaginator)
3. item: [:material-code-braces: GetOutpostInstanceTypesOutputTypeDef](./type_defs.md#getoutpostinstancetypesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[outposts]`
or a standalone `types_aiobotocore_outposts` package, you have to explicitly specify
`client: OutpostsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OutpostsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_outposts.client import OutpostsClient
from types_aiobotocore_outposts.type_defs import CreateOrderOutputTypeDef
from types_aiobotocore_outposts.type_defs import CreateOrderInputTypeDef


session = get_session()

async with session.create_client("outposts") as client:
    client: OutpostsClient
    kwargs: CreateOrderInputTypeDef = {...}
    result: CreateOrderOutputTypeDef = await client.create_order(**kwargs)
```



```python
# GetOutpostInstanceTypesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_outposts.client import OutpostsClient
from types_aiobotocore_outposts.paginator import GetOutpostInstanceTypesPaginator
from types_aiobotocore_outposts.type_defs import GetOutpostInstanceTypesOutputTypeDef


session = get_session()

async with session.create_client("outposts") as client:
    client: OutpostsClient
    paginator: GetOutpostInstanceTypesPaginator = client.get_paginator("get_outpost_instance_types")
    async for item in paginator.paginate(...):
        item: GetOutpostInstanceTypesOutputTypeDef
        print(item)
```


