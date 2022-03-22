<a id="examples-for-aiobotocore-swf-module"></a>

# Examples for aiobotocore SWF module

> [Index](../README.md) > [SWF](./README.md) > Examples

- [Examples for aiobotocore SWF module](#examples-for-aiobotocore-swf-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[swf]` package installed.

Write your `SWF` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SWFClient
# and provides type checking and code completion
async with session.create_client("swf") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetWorkflowExecutionHistoryPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_workflow_execution_history")
    async for item in paginator.paginate(...):
        # item has type HistoryTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[swf]` or a standalone `types_aiobotocore_swf`
package, you have to explicitly specify `client: SWFClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.client import SWFClient
from types_aiobotocore_swf.type_defs import bool
from types_aiobotocore_swf.paginator import GetWorkflowExecutionHistoryPaginator

from types_aiobotocore_swf.literals import PaginatorName



session = get_session()

async with session.create_client("swf") as client:
    client: SWFClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_workflow_execution_history"
    paginator: GetWorkflowExecutionHistoryPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: HistoryTypeDef
        print(item)
    

    
```
