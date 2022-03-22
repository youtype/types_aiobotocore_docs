<a id="examples-for-aiobotocore-polly-module"></a>

# Examples for aiobotocore Polly module

> [Index](../README.md) > [Polly](./README.md) > Examples

- [Examples for aiobotocore Polly module](#examples-for-aiobotocore-polly-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[polly]` package installed.

Write your `Polly` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PollyClient
# and provides type checking and code completion
async with session.create_client("polly") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeVoicesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_voices")
    async for item in paginator.paginate(...):
        # item has type DescribeVoicesOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[polly]` or a standalone `types_aiobotocore_polly`
package, you have to explicitly specify `client: PollyClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_polly.client import PollyClient
from types_aiobotocore_polly.type_defs import bool
from types_aiobotocore_polly.paginator import DescribeVoicesPaginator

from types_aiobotocore_polly.literals import PaginatorName



session = get_session()

async with session.create_client("polly") as client:
    client: PollyClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_voices"
    paginator: DescribeVoicesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeVoicesOutputTypeDef
        print(item)
    

    
```
