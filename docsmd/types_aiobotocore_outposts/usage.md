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



#### Client method usage example

```python
# OutpostsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("outposts") as client:  # (1)
    result = await client.create_order()  # (2)
```

1. client: [OutpostsClient](./client.md)
2. result: [:material-code-braces: CreateOrderOutputTypeDef](./type_defs.md#createorderoutputtypedef)



#### Paginator usage example

```python
# GetOutpostBillingInformationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("outposts") as client:  # (1)
    paginator = client.get_paginator("get_outpost_billing_information")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [GetOutpostBillingInformationPaginator](./paginators.md#getoutpostbillinginformationpaginator)
3. item: [:material-code-braces: GetOutpostBillingInformationOutputTypeDef](./type_defs.md#getoutpostbillinginformationoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[outposts]`
or a standalone `types_aiobotocore_outposts` package, you have to explicitly specify
`client: OutpostsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

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



#### Paginator usage example

```python
# GetOutpostBillingInformationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_outposts.client import OutpostsClient
from types_aiobotocore_outposts.paginator import GetOutpostBillingInformationPaginator
from types_aiobotocore_outposts.type_defs import GetOutpostBillingInformationOutputTypeDef


session = get_session()

async with session.create_client("outposts") as client:
    client: OutpostsClient
    paginator: GetOutpostBillingInformationPaginator = client.get_paginator("get_outpost_billing_information")
    async for item in paginator.paginate(...):
        item: GetOutpostBillingInformationOutputTypeDef
        print(item)
```


