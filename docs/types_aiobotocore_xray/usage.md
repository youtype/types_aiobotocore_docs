<a id="examples-for-aiobotocore-xray-module"></a>

# Examples for aiobotocore XRay module

> [Index](../README.md) > [XRay](./README.md) > Examples

- [Examples for aiobotocore XRay module](#examples-for-aiobotocore-xray-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[xray]` package installed.

Write your `XRay` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type XRayClient
# and provides type checking and code completion
async with session.create_client("xray") as client:
    
    # result has type BatchGetTracesResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_get_traces()
    

    
    # paginator has type BatchGetTracesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("batch_get_traces")
    async for item in paginator.paginate(...):
        # item has type BatchGetTracesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[xray]` or a standalone `types_aiobotocore_xray`
package, you have to explicitly specify `client: XRayClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_xray.client import XRayClient
from types_aiobotocore_xray.type_defs import BatchGetTracesResultTypeDef
from types_aiobotocore_xray.paginator import BatchGetTracesPaginator

from types_aiobotocore_xray.literals import PaginatorName



session = get_session()

async with session.create_client("xray") as client:
    client: XRayClient

    
    result: BatchGetTracesResultTypeDef = client.batch_get_traces()
    

    
    paginator_name: PaginatorName = "batch_get_traces"
    paginator: BatchGetTracesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: BatchGetTracesResultTypeDef
        print(item)
    

    
```
