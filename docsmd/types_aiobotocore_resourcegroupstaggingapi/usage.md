# Examples

> [Index](../README.md) > [ResourceGroupsTaggingAPI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#resourcegroupstaggingapi)
    type annotations stubs module [types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[resourcegroupstaggingapi]` package installed.

Write your `ResourceGroupsTaggingAPI` code as usual,
type checking and code completion should work out of the box.



```python
# ResourceGroupsTaggingAPIClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resourcegroupstaggingapi") as client:  # (1)
    result = await client.get_compliance_summary()  # (2)
```

1. client: [ResourceGroupsTaggingAPIClient](./client.md)
2. result: [:material-code-braces: GetComplianceSummaryOutputTypeDef](./type_defs.md#getcompliancesummaryoutputtypedef) 



```python
# GetComplianceSummaryPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resourcegroupstaggingapi") as client:  # (1)
    paginator = client.get_paginator("get_compliance_summary")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ResourceGroupsTaggingAPIClient](./client.md)
2. paginator: [GetComplianceSummaryPaginator](./paginators.md#getcompliancesummarypaginator)
3. item: [:material-code-braces: GetComplianceSummaryOutputTypeDef](./type_defs.md#getcompliancesummaryoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[resourcegroupstaggingapi]`
or a standalone `types_aiobotocore_resourcegroupstaggingapi` package, you have to explicitly specify
`client: ResourceGroupsTaggingAPIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ResourceGroupsTaggingAPIClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient
from types_aiobotocore_resourcegroupstaggingapi.type_defs import GetComplianceSummaryOutputTypeDef
from types_aiobotocore_resourcegroupstaggingapi.type_defs import GetComplianceSummaryInputTypeDef


session = get_session()

async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
    kwargs: GetComplianceSummaryInputTypeDef = {...}
    result: GetComplianceSummaryOutputTypeDef = await client.get_compliance_summary(**kwargs)
```



```python
# GetComplianceSummaryPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient
from types_aiobotocore_resourcegroupstaggingapi.paginator import GetComplianceSummaryPaginator
from types_aiobotocore_resourcegroupstaggingapi.type_defs import GetComplianceSummaryOutputTypeDef


session = get_session()

async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
    paginator: GetComplianceSummaryPaginator = client.get_paginator("get_compliance_summary")
    async for item in paginator.paginate(...):
        item: GetComplianceSummaryOutputTypeDef
        print(item)
```


