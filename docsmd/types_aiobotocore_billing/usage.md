# Examples

> [Index](../README.md) > [Billing](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[billing]` package installed.

Write your `Billing` code as usual,
type checking and code completion should work out of the box.



```python
# BillingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("billing") as client:  # (1)
    result = await client.create_billing_view()  # (2)
```

1. client: [BillingClient](./client.md)
2. result: [:material-code-braces: CreateBillingViewResponseTypeDef](./type_defs.md#createbillingviewresponsetypedef) 



```python
# ListBillingViewsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("billing") as client:  # (1)
    paginator = client.get_paginator("list_billing_views")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BillingClient](./client.md)
2. paginator: [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)
3. item: [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[billing]`
or a standalone `types_aiobotocore_billing` package, you have to explicitly specify
`client: BillingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BillingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_billing.client import BillingClient
from types_aiobotocore_billing.type_defs import CreateBillingViewResponseTypeDef
from types_aiobotocore_billing.type_defs import CreateBillingViewRequestTypeDef


session = get_session()

async with session.create_client("billing") as client:
    client: BillingClient
    kwargs: CreateBillingViewRequestTypeDef = {...}
    result: CreateBillingViewResponseTypeDef = await client.create_billing_view(**kwargs)
```



```python
# ListBillingViewsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_billing.client import BillingClient
from types_aiobotocore_billing.paginator import ListBillingViewsPaginator
from types_aiobotocore_billing.type_defs import ListBillingViewsResponseTypeDef


session = get_session()

async with session.create_client("billing") as client:
    client: BillingClient
    paginator: ListBillingViewsPaginator = client.get_paginator("list_billing_views")
    async for item in paginator.paginate(...):
        item: ListBillingViewsResponseTypeDef
        print(item)
```


