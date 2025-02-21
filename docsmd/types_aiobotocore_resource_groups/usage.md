# Examples

> [Index](../README.md) > [ResourceGroups](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#resourcegroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[resource-groups]` package installed.

Write your `ResourceGroups` code as usual,
type checking and code completion should work out of the box.



```python
# ResourceGroupsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resource-groups") as client:  # (1)
    result = await client.cancel_tag_sync_task()  # (2)
```

1. client: [ResourceGroupsClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListGroupResourcesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("resource-groups") as client:  # (1)
    paginator = client.get_paginator("list_group_resources")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ResourceGroupsClient](./client.md)
2. paginator: [ListGroupResourcesPaginator](./paginators.md#listgroupresourcespaginator)
3. item: [:material-code-braces: ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[resource-groups]`
or a standalone `types_aiobotocore_resource_groups` package, you have to explicitly specify
`client: ResourceGroupsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ResourceGroupsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.client import ResourceGroupsClient
from types_aiobotocore_resource_groups.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_resource_groups.type_defs import CancelTagSyncTaskInputTypeDef


session = get_session()

async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient
    kwargs: CancelTagSyncTaskInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.cancel_tag_sync_task(**kwargs)
```



```python
# ListGroupResourcesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.client import ResourceGroupsClient
from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator
from types_aiobotocore_resource_groups.type_defs import ListGroupResourcesOutputTypeDef


session = get_session()

async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient
    paginator: ListGroupResourcesPaginator = client.get_paginator("list_group_resources")
    async for item in paginator.paginate(...):
        item: ListGroupResourcesOutputTypeDef
        print(item)
```


