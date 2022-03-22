<a id="examples-for-aiobotocore-resourcegroupstaggingapi-module"></a>

# Examples for aiobotocore ResourceGroupsTaggingAPI module

> [Index](../README.md) > [ResourceGroupsTaggingAPI](./README.md) > Examples

- [Examples for aiobotocore ResourceGroupsTaggingAPI module](#examples-for-aiobotocore-resourcegroupstaggingapi-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[resourcegroupstaggingapi]` package
installed.

Write your `ResourceGroupsTaggingAPI` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ResourceGroupsTaggingAPIClient
# and provides type checking and code completion
async with session.create_client("resourcegroupstaggingapi") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetComplianceSummaryPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_compliance_summary")
    async for item in paginator.paginate(...):
        # item has type GetComplianceSummaryOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[resourcegroupstaggingapi]` or a standalone
`types_aiobotocore_resourcegroupstaggingapi` package, you have to explicitly
specify `client: ResourceGroupsTaggingAPIClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient
from types_aiobotocore_resourcegroupstaggingapi.type_defs import bool
from types_aiobotocore_resourcegroupstaggingapi.paginator import GetComplianceSummaryPaginator

from types_aiobotocore_resourcegroupstaggingapi.literals import PaginatorName



session = get_session()

async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_compliance_summary"
    paginator: GetComplianceSummaryPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetComplianceSummaryOutputTypeDef
        print(item)
    

    
```
