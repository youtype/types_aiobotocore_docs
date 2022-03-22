<a id="examples-for-aiobotocore-pricing-module"></a>

# Examples for aiobotocore Pricing module

> [Index](../README.md) > [Pricing](./README.md) > Examples

- [Examples for aiobotocore Pricing module](#examples-for-aiobotocore-pricing-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[pricing]` package installed.

Write your `Pricing` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PricingClient
# and provides type checking and code completion
async with session.create_client("pricing") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeServicesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_services")
    async for item in paginator.paginate(...):
        # item has type DescribeServicesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[pricing]` or a standalone
`types_aiobotocore_pricing` package, you have to explicitly specify
`client: PricingClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_pricing.client import PricingClient
from types_aiobotocore_pricing.type_defs import bool
from types_aiobotocore_pricing.paginator import DescribeServicesPaginator

from types_aiobotocore_pricing.literals import PaginatorName



session = get_session()

async with session.create_client("pricing") as client:
    client: PricingClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_services"
    paginator: DescribeServicesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeServicesResponseTypeDef
        print(item)
    

    
```
