<a id="examples-for-aiobotocore-greengrass-module"></a>

# Examples for aiobotocore Greengrass module

> [Index](../README.md) > [Greengrass](./README.md) > Examples

- [Examples for aiobotocore Greengrass module](#examples-for-aiobotocore-greengrass-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[greengrass]` package installed.

Write your `Greengrass` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GreengrassClient
# and provides type checking and code completion
async with session.create_client("greengrass") as client:
    
    # result has type AssociateRoleToGroupResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_role_to_group()
    

    
    # paginator has type ListBulkDeploymentDetailedReportsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_bulk_deployment_detailed_reports")
    async for item in paginator.paginate(...):
        # item has type ListBulkDeploymentDetailedReportsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[greengrass]` or a standalone
`types_aiobotocore_greengrass` package, you have to explicitly specify
`client: GreengrassClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_greengrass.client import GreengrassClient
from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupResponseTypeDef
from types_aiobotocore_greengrass.paginator import ListBulkDeploymentDetailedReportsPaginator

from types_aiobotocore_greengrass.literals import PaginatorName



session = get_session()

async with session.create_client("greengrass") as client:
    client: GreengrassClient

    
    result: AssociateRoleToGroupResponseTypeDef = client.associate_role_to_group()
    

    
    paginator_name: PaginatorName = "list_bulk_deployment_detailed_reports"
    paginator: ListBulkDeploymentDetailedReportsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListBulkDeploymentDetailedReportsResponseTypeDef
        print(item)
    

    
```
