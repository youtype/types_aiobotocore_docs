<a id="paginators-for-aiobotocore-costandusagereportservice-module"></a>

# Paginators for aiobotocore CostandUsageReportService module

> [Index](../README.md) > [CostandUsageReportService](./README.md) > Paginators

Auto-generated documentation for
[CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
type annotations stubs module
[types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

- [Paginators for aiobotocore CostandUsageReportService module](#paginators-for-aiobotocore-costandusagereportservice-module)
  - [DescribeReportDefinitionsPaginator](#describereportdefinitionspaginator)

<a id="describereportdefinitionspaginator"></a>

## DescribeReportDefinitionsPaginator

Type annotations for
`session.create_client("cur").get_paginator("describe_report_definitions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator

session = get_session()
async with session.create_client("cur") as client:
    client: CostandUsageReportServiceClient
    paginator: DescribeReportDefinitionsPaginator = client.get_paginator("describe_report_definitions")
```

Boto3 documentation:
[CostandUsageReportService.Paginator.DescribeReportDefinitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)

Arguments for `DescribeReportDefinitionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReportDefinitionsPaginator.paginate` returns
`AsyncIterator`\[[DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef)\].