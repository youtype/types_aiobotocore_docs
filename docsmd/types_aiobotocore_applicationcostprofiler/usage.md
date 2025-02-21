# Examples

> [Index](../README.md) > [ApplicationCostProfiler](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#applicationcostprofiler)
    type annotations stubs module [types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[applicationcostprofiler]` package installed.

Write your `ApplicationCostProfiler` code as usual,
type checking and code completion should work out of the box.



```python
# ApplicationCostProfilerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("applicationcostprofiler") as client:  # (1)
    result = await client.delete_report_definition()  # (2)
```

1. client: [ApplicationCostProfilerClient](./client.md)
2. result: [:material-code-braces: DeleteReportDefinitionResultTypeDef](./type_defs.md#deletereportdefinitionresulttypedef) 



```python
# ListReportDefinitionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("applicationcostprofiler") as client:  # (1)
    paginator = client.get_paginator("list_report_definitions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ApplicationCostProfilerClient](./client.md)
2. paginator: [ListReportDefinitionsPaginator](./paginators.md#listreportdefinitionspaginator)
3. item: [:material-code-braces: ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[applicationcostprofiler]`
or a standalone `types_aiobotocore_applicationcostprofiler` package, you have to explicitly specify
`client: ApplicationCostProfilerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ApplicationCostProfilerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_applicationcostprofiler.client import ApplicationCostProfilerClient
from types_aiobotocore_applicationcostprofiler.type_defs import DeleteReportDefinitionResultTypeDef
from types_aiobotocore_applicationcostprofiler.type_defs import DeleteReportDefinitionRequestTypeDef


session = get_session()

async with session.create_client("applicationcostprofiler") as client:
    client: ApplicationCostProfilerClient
    kwargs: DeleteReportDefinitionRequestTypeDef = {...}
    result: DeleteReportDefinitionResultTypeDef = await client.delete_report_definition(**kwargs)
```



```python
# ListReportDefinitionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_applicationcostprofiler.client import ApplicationCostProfilerClient
from types_aiobotocore_applicationcostprofiler.paginator import ListReportDefinitionsPaginator
from types_aiobotocore_applicationcostprofiler.type_defs import ListReportDefinitionsResultTypeDef


session = get_session()

async with session.create_client("applicationcostprofiler") as client:
    client: ApplicationCostProfilerClient
    paginator: ListReportDefinitionsPaginator = client.get_paginator("list_report_definitions")
    async for item in paginator.paginate(...):
        item: ListReportDefinitionsResultTypeDef
        print(item)
```


