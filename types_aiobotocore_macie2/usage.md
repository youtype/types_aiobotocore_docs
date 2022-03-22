<a id="examples-for-aiobotocore-macie2-module"></a>

# Examples for aiobotocore Macie2 module

> [Index](../README.md) > [Macie2](./README.md) > Examples

- [Examples for aiobotocore Macie2 module](#examples-for-aiobotocore-macie2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[macie2]` package installed.

Write your `Macie2` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Macie2Client
# and provides type checking and code completion
async with session.create_client("macie2") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_invitation()
    

    
    # paginator has type DescribeBucketsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_buckets")
    async for item in paginator.paginate(...):
        # item has type DescribeBucketsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[macie2]` or a standalone
`types_aiobotocore_macie2` package, you have to explicitly specify
`client: Macie2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_macie2.client import Macie2Client
from types_aiobotocore_macie2.type_defs import Dict[str, Any]
from types_aiobotocore_macie2.paginator import DescribeBucketsPaginator

from types_aiobotocore_macie2.literals import PaginatorName



session = get_session()

async with session.create_client("macie2") as client:
    client: Macie2Client

    
    result: Dict[str, Any] = client.accept_invitation()
    

    
    paginator_name: PaginatorName = "describe_buckets"
    paginator: DescribeBucketsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeBucketsResponseTypeDef
        print(item)
    

    
```
