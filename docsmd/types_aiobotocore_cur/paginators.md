# Paginators

> [Index](../README.md) > [CostandUsageReportService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## DescribeReportDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("cur").get_paginator("describe_report_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator

session = get_session()
async with session.create_client("cur") as client:
    client: CostandUsageReportServiceClient
    paginator: DescribeReportDefinitionsPaginator = client.get_paginator("describe_report_definitions")
```


### paginate

Type annotations and code completion for `#!python DescribeReportDefinitionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReportDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef](./type_defs.md#describereportdefinitionsrequestdescribereportdefinitionspaginatetypedef) 
