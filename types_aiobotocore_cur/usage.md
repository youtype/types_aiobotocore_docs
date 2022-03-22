<a id="examples-for-aiobotocore-costandusagereportservice-module"></a>

# Examples for aiobotocore CostandUsageReportService module

> [Index](../README.md) > [CostandUsageReportService](./README.md) > Examples

- [Examples for aiobotocore CostandUsageReportService module](#examples-for-aiobotocore-costandusagereportservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cur]` package installed.

Write your `CostandUsageReportService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CostandUsageReportServiceClient
# and provides type checking and code completion
async with session.create_client("cur") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeReportDefinitionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_report_definitions")
    async for item in paginator.paginate(...):
        # item has type DescribeReportDefinitionsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cur]` or a standalone `types_aiobotocore_cur`
package, you have to explicitly specify
`client: CostandUsageReportServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cur.client import CostandUsageReportServiceClient
from types_aiobotocore_cur.type_defs import bool
from types_aiobotocore_cur.paginator import DescribeReportDefinitionsPaginator

from types_aiobotocore_cur.literals import PaginatorName



session = get_session()

async with session.create_client("cur") as client:
    client: CostandUsageReportServiceClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_report_definitions"
    paginator: DescribeReportDefinitionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeReportDefinitionsResponseTypeDef
        print(item)
    

    
```
