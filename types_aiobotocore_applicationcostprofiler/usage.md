<a id="examples-for-aiobotocore-applicationcostprofiler-module"></a>

# Examples for aiobotocore ApplicationCostProfiler module

> [Index](../README.md) > [ApplicationCostProfiler](./README.md) > Examples

- [Examples for aiobotocore ApplicationCostProfiler module](#examples-for-aiobotocore-applicationcostprofiler-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[applicationcostprofiler]` package
installed.

Write your `ApplicationCostProfiler` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ApplicationCostProfilerClient
# and provides type checking and code completion
async with session.create_client("applicationcostprofiler") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListReportDefinitionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_report_definitions")
    async for item in paginator.paginate(...):
        # item has type ListReportDefinitionsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[applicationcostprofiler]` or a standalone
`types_aiobotocore_applicationcostprofiler` package, you have to explicitly
specify `client: ApplicationCostProfilerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_applicationcostprofiler.client import ApplicationCostProfilerClient
from types_aiobotocore_applicationcostprofiler.type_defs import bool
from types_aiobotocore_applicationcostprofiler.paginator import ListReportDefinitionsPaginator

from types_aiobotocore_applicationcostprofiler.literals import PaginatorName



session = get_session()

async with session.create_client("applicationcostprofiler") as client:
    client: ApplicationCostProfilerClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_report_definitions"
    paginator: ListReportDefinitionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListReportDefinitionsResultTypeDef
        print(item)
    

    
```
