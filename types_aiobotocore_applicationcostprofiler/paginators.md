<a id="paginators-for-aiobotocore-applicationcostprofiler-module"></a>

# Paginators for aiobotocore ApplicationCostProfiler module

> [Index](..) > [ApplicationCostProfiler](.) > Paginators

Auto-generated documentation for
[ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
type annotations stubs module
[types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).

- [Paginators for aiobotocore ApplicationCostProfiler module](#paginators-for-aiobotocore-applicationcostprofiler-module)
  - [ListReportDefinitionsPaginator](#listreportdefinitionspaginator)

<a id="listreportdefinitionspaginator"></a>

## ListReportDefinitionsPaginator

Type annotations for
`aiobotocore.create_client("applicationcostprofiler").get_paginator("list_report_definitions")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_applicationcostprofiler.paginator import ListReportDefinitionsPaginator

def get_list_report_definitions_paginator() -> ListReportDefinitionsPaginator:
    return Session().create_client("applicationcostprofiler").get_paginator("list_report_definitions")
```

Boto3 documentation:
[ApplicationCostProfiler.Paginator.ListReportDefinitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions)

Arguments for `ListReportDefinitionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReportDefinitionsPaginator.paginate` returns
`_PageIterator`\[[ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef)\].
