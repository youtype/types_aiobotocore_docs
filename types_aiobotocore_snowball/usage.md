<a id="examples-for-aiobotocore-snowball-module"></a>

# Examples for aiobotocore Snowball module

> [Index](../README.md) > [Snowball](./README.md) > Examples

- [Examples for aiobotocore Snowball module](#examples-for-aiobotocore-snowball-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[snowball]` package installed.

Write your `Snowball` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SnowballClient
# and provides type checking and code completion
async with session.create_client("snowball") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeAddressesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_addresses")
    async for item in paginator.paginate(...):
        # item has type DescribeAddressesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[snowball]` or a standalone
`types_aiobotocore_snowball` package, you have to explicitly specify
`client: SnowballClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_snowball.client import SnowballClient
from types_aiobotocore_snowball.type_defs import bool
from types_aiobotocore_snowball.paginator import DescribeAddressesPaginator

from types_aiobotocore_snowball.literals import PaginatorName



session = get_session()

async with session.create_client("snowball") as client:
    client: SnowballClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_addresses"
    paginator: DescribeAddressesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAddressesResultTypeDef
        print(item)
    

    
```
