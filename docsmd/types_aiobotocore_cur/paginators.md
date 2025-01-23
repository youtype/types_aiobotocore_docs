# Paginators

> [Index](../README.md) > [CostandUsageReportService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#costandusagereportservice)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## DescribeReportDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("cur").get_paginator("describe_report_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/paginator/DescribeReportDefinitions.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)

```python
# DescribeReportDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator

session = get_session()
async with session.create_client("cur") as client:  # (1)
    paginator: DescribeReportDefinitionsPaginator = client.get_paginator("describe_report_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReportDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [CostandUsageReportServiceClient](./client.md)
2. paginator: [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)
3. item: [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReportDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeReportDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReportDefinitionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReportDefinitionsRequestPaginateTypeDef](./type_defs.md#describereportdefinitionsrequestpaginatetypedef) 
