# Examples

> [Index](../README.md) > [Greengrass](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Greengrass](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#greengrass)
    type annotations stubs module [types-aiobotocore-greengrass](https://pypi.org/project/types-aiobotocore-greengrass/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[greengrass]` package installed.

Write your `Greengrass` code as usual,
type checking and code completion should work out of the box.



```python
# GreengrassClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("greengrass") as client:  # (1)
    result = await client.associate_role_to_group()  # (2)
```

1. client: [GreengrassClient](./client.md)
2. result: [:material-code-braces: AssociateRoleToGroupResponseTypeDef](./type_defs.md#associateroletogroupresponsetypedef) 



```python
# ListBulkDeploymentDetailedReportsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("greengrass") as client:  # (1)
    paginator = client.get_paginator("list_bulk_deployment_detailed_reports")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [GreengrassClient](./client.md)
2. paginator: [ListBulkDeploymentDetailedReportsPaginator](./paginators.md#listbulkdeploymentdetailedreportspaginator)
3. item: [:material-code-braces: ListBulkDeploymentDetailedReportsResponseTypeDef](./type_defs.md#listbulkdeploymentdetailedreportsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[greengrass]`
or a standalone `types_aiobotocore_greengrass` package, you have to explicitly specify
`client: GreengrassClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# GreengrassClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.client import GreengrassClient
from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupResponseTypeDef
from types_aiobotocore_greengrass.type_defs import AssociateRoleToGroupRequestTypeDef


session = get_session()

async with session.create_client("greengrass") as client:
    client: GreengrassClient
    kwargs: AssociateRoleToGroupRequestTypeDef = {...}
    result: AssociateRoleToGroupResponseTypeDef = await client.associate_role_to_group(**kwargs)
```



```python
# ListBulkDeploymentDetailedReportsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_greengrass.client import GreengrassClient
from types_aiobotocore_greengrass.paginator import ListBulkDeploymentDetailedReportsPaginator
from types_aiobotocore_greengrass.type_defs import ListBulkDeploymentDetailedReportsResponseTypeDef


session = get_session()

async with session.create_client("greengrass") as client:
    client: GreengrassClient
    paginator: ListBulkDeploymentDetailedReportsPaginator = client.get_paginator("list_bulk_deployment_detailed_reports")
    async for item in paginator.paginate(...):
        item: ListBulkDeploymentDetailedReportsResponseTypeDef
        print(item)
```


