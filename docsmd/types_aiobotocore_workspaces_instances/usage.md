# Examples

> [Index](../README.md) > [WorkspacesInstances](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkspacesInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances.html#workspacesinstances)
    type annotations stubs module [types-aiobotocore-workspaces-instances](https://pypi.org/project/types-aiobotocore-workspaces-instances/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[workspaces-instances]` package installed.

Write your `WorkspacesInstances` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# WorkspacesInstancesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces-instances") as client:  # (1)
    result = await client.create_volume()  # (2)
```

1. client: [WorkspacesInstancesClient](./client.md)
2. result: [:material-code-braces: CreateVolumeResponseTypeDef](./type_defs.md#createvolumeresponsetypedef)



#### Paginator usage example

```python
# ListInstanceTypesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces-instances") as client:  # (1)
    paginator = client.get_paginator("list_instance_types")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkspacesInstancesClient](./client.md)
2. paginator: [ListInstanceTypesPaginator](./paginators.md#listinstancetypespaginator)
3. item: [:material-code-braces: ListInstanceTypesResponseTypeDef](./type_defs.md#listinstancetypesresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[workspaces-instances]`
or a standalone `types_aiobotocore_workspaces_instances` package, you have to explicitly specify
`client: WorkspacesInstancesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# WorkspacesInstancesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_instances.client import WorkspacesInstancesClient
from types_aiobotocore_workspaces_instances.type_defs import CreateVolumeResponseTypeDef
from types_aiobotocore_workspaces_instances.type_defs import CreateVolumeRequestTypeDef


session = get_session()

async with session.create_client("workspaces-instances") as client:
    client: WorkspacesInstancesClient
    kwargs: CreateVolumeRequestTypeDef = {...}
    result: CreateVolumeResponseTypeDef = await client.create_volume(**kwargs)
```



#### Paginator usage example

```python
# ListInstanceTypesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_instances.client import WorkspacesInstancesClient
from types_aiobotocore_workspaces_instances.paginator import ListInstanceTypesPaginator
from types_aiobotocore_workspaces_instances.type_defs import ListInstanceTypesResponseTypeDef


session = get_session()

async with session.create_client("workspaces-instances") as client:
    client: WorkspacesInstancesClient
    paginator: ListInstanceTypesPaginator = client.get_paginator("list_instance_types")
    async for item in paginator.paginate(...):
        item: ListInstanceTypesResponseTypeDef
        print(item)
```


