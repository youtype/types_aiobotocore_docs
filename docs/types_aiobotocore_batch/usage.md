<a id="examples-for-aiobotocore-batch-module"></a>

# Examples for aiobotocore Batch module

> [Index](../README.md) > [Batch](./README.md) > Examples

- [Examples for aiobotocore Batch module](#examples-for-aiobotocore-batch-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[batch]` package installed.

Write your `Batch` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type BatchClient
# and provides type checking and code completion
async with session.create_client("batch") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeComputeEnvironmentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_compute_environments")
    async for item in paginator.paginate(...):
        # item has type DescribeComputeEnvironmentsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[batch]` or a standalone `types_aiobotocore_batch`
package, you have to explicitly specify `client: BatchClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_batch.client import BatchClient
from types_aiobotocore_batch.type_defs import bool
from types_aiobotocore_batch.paginator import DescribeComputeEnvironmentsPaginator

from types_aiobotocore_batch.literals import PaginatorName



session = get_session()

async with session.create_client("batch") as client:
    client: BatchClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_compute_environments"
    paginator: DescribeComputeEnvironmentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeComputeEnvironmentsResponseTypeDef
        print(item)
    

    
```
