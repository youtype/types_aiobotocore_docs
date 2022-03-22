<a id="examples-for-aiobotocore-drs-module"></a>

# Examples for aiobotocore drs module

> [Index](../README.md) > [drs](./README.md) > Examples

- [Examples for aiobotocore drs module](#examples-for-aiobotocore-drs-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[drs]` package installed.

Write your `drs` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type drsClient
# and provides type checking and code completion
async with session.create_client("drs") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeJobLogItemsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_job_log_items")
    async for item in paginator.paginate(...):
        # item has type DescribeJobLogItemsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[drs]` or a standalone `types_aiobotocore_drs`
package, you have to explicitly specify `client: drsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_drs.client import drsClient
from types_aiobotocore_drs.type_defs import bool
from types_aiobotocore_drs.paginator import DescribeJobLogItemsPaginator

from types_aiobotocore_drs.literals import PaginatorName



session = get_session()

async with session.create_client("drs") as client:
    client: drsClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_job_log_items"
    paginator: DescribeJobLogItemsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeJobLogItemsResponseTypeDef
        print(item)
    

    
```
