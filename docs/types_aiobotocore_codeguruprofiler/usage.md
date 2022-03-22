<a id="examples-for-aiobotocore-codeguruprofiler-module"></a>

# Examples for aiobotocore CodeGuruProfiler module

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > Examples

- [Examples for aiobotocore CodeGuruProfiler module](#examples-for-aiobotocore-codeguruprofiler-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codeguruprofiler]` package installed.

Write your `CodeGuruProfiler` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeGuruProfilerClient
# and provides type checking and code completion
async with session.create_client("codeguruprofiler") as client:
    
    # result has type AddNotificationChannelsResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_notification_channels()
    

    
    # paginator has type ListProfileTimesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_profile_times")
    async for item in paginator.paginate(...):
        # item has type ListProfileTimesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codeguruprofiler]` or a standalone
`types_aiobotocore_codeguruprofiler` package, you have to explicitly specify
`client: CodeGuruProfilerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeguruprofiler.client import CodeGuruProfilerClient
from types_aiobotocore_codeguruprofiler.type_defs import AddNotificationChannelsResponseTypeDef
from types_aiobotocore_codeguruprofiler.paginator import ListProfileTimesPaginator

from types_aiobotocore_codeguruprofiler.literals import PaginatorName



session = get_session()

async with session.create_client("codeguruprofiler") as client:
    client: CodeGuruProfilerClient

    
    result: AddNotificationChannelsResponseTypeDef = client.add_notification_channels()
    

    
    paginator_name: PaginatorName = "list_profile_times"
    paginator: ListProfileTimesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListProfileTimesResponseTypeDef
        print(item)
    

    
```
