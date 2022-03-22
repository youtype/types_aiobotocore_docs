<a id="examples-for-aiobotocore-quicksight-module"></a>

# Examples for aiobotocore QuickSight module

> [Index](../README.md) > [QuickSight](./README.md) > Examples

- [Examples for aiobotocore QuickSight module](#examples-for-aiobotocore-quicksight-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[quicksight]` package installed.

Write your `QuickSight` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type QuickSightClient
# and provides type checking and code completion
async with session.create_client("quicksight") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAnalysesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_analyses")
    async for item in paginator.paginate(...):
        # item has type ListAnalysesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[quicksight]` or a standalone
`types_aiobotocore_quicksight` package, you have to explicitly specify
`client: QuickSightClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_quicksight.client import QuickSightClient
from types_aiobotocore_quicksight.type_defs import bool
from types_aiobotocore_quicksight.paginator import ListAnalysesPaginator

from types_aiobotocore_quicksight.literals import PaginatorName



session = get_session()

async with session.create_client("quicksight") as client:
    client: QuickSightClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_analyses"
    paginator: ListAnalysesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAnalysesResponseTypeDef
        print(item)
    

    
```
