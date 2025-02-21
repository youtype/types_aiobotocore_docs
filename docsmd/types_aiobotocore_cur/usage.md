# Examples

> [Index](../README.md) > [CostandUsageReportService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#costandusagereportservice)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cur]` package installed.

Write your `CostandUsageReportService` code as usual,
type checking and code completion should work out of the box.



```python
# CostandUsageReportServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cur") as client:  # (1)
    result = await client.delete_report_definition()  # (2)
```

1. client: [CostandUsageReportServiceClient](./client.md)
2. result: [:material-code-braces: DeleteReportDefinitionResponseTypeDef](./type_defs.md#deletereportdefinitionresponsetypedef) 



```python
# DescribeReportDefinitionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cur") as client:  # (1)
    paginator = client.get_paginator("describe_report_definitions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CostandUsageReportServiceClient](./client.md)
2. paginator: [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)
3. item: [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[cur]`
or a standalone `types_aiobotocore_cur` package, you have to explicitly specify
`client: CostandUsageReportServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CostandUsageReportServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cur.client import CostandUsageReportServiceClient
from types_aiobotocore_cur.type_defs import DeleteReportDefinitionResponseTypeDef
from types_aiobotocore_cur.type_defs import DeleteReportDefinitionRequestTypeDef


session = get_session()

async with session.create_client("cur") as client:
    client: CostandUsageReportServiceClient
    kwargs: DeleteReportDefinitionRequestTypeDef = {...}
    result: DeleteReportDefinitionResponseTypeDef = await client.delete_report_definition(**kwargs)
```



```python
# DescribeReportDefinitionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cur.client import CostandUsageReportServiceClient
from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator
from types_aiobotocore_cur.type_defs import DescribeReportDefinitionsResponseTypeDef


session = get_session()

async with session.create_client("cur") as client:
    client: CostandUsageReportServiceClient
    paginator: DescribeReportDefinitionsPaginator = client.get_paginator("describe_report_definitions")
    async for item in paginator.paginate(...):
        item: DescribeReportDefinitionsResponseTypeDef
        print(item)
```


