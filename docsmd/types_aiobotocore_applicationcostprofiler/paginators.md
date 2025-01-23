# Paginators

> [Index](../README.md) > [ApplicationCostProfiler](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#applicationcostprofiler)
    type annotations stubs module [types-aiobotocore-applicationcostprofiler](https://pypi.org/project/types-aiobotocore-applicationcostprofiler/).

## ListReportDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("applicationcostprofiler").get_paginator("list_report_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler/paginator/ListReportDefinitions.html#ApplicationCostProfiler.Paginator.ListReportDefinitions)

```python
# ListReportDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_applicationcostprofiler.paginator import ListReportDefinitionsPaginator

session = get_session()
async with session.create_client("applicationcostprofiler") as client:  # (1)
    paginator: ListReportDefinitionsPaginator = client.get_paginator("list_report_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListReportDefinitionsResultTypeDef
        print(item)  # (3)
```

1. client: [ApplicationCostProfilerClient](./client.md)
2. paginator: [ListReportDefinitionsPaginator](./paginators.md#listreportdefinitionspaginator)
3. item: [:material-code-braces: ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListReportDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListReportDefinitionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReportDefinitionsResultTypeDef](./type_defs.md#listreportdefinitionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListReportDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReportDefinitionsRequestPaginateTypeDef](./type_defs.md#listreportdefinitionsrequestpaginatetypedef) 
