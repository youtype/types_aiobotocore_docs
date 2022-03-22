<a id="examples-for-aiobotocore-dax-module"></a>

# Examples for aiobotocore DAX module

> [Index](../README.md) > [DAX](./README.md) > Examples

- [Examples for aiobotocore DAX module](#examples-for-aiobotocore-dax-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[dax]` package installed.

Write your `DAX` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DAXClient
# and provides type checking and code completion
async with session.create_client("dax") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeClustersPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_clusters")
    async for item in paginator.paginate(...):
        # item has type DescribeClustersResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[dax]` or a standalone `types_aiobotocore_dax`
package, you have to explicitly specify `client: DAXClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.client import DAXClient
from types_aiobotocore_dax.type_defs import bool
from types_aiobotocore_dax.paginator import DescribeClustersPaginator

from types_aiobotocore_dax.literals import PaginatorName



session = get_session()

async with session.create_client("dax") as client:
    client: DAXClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_clusters"
    paginator: DescribeClustersPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeClustersResponseTypeDef
        print(item)
    

    
```
