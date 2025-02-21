# Examples

> [Index](../README.md) > [Neptune](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#neptune)
    type annotations stubs module [types-aiobotocore-neptune](https://pypi.org/project/types-aiobotocore-neptune/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[neptune]` package installed.

Write your `Neptune` code as usual,
type checking and code completion should work out of the box.



```python
# NeptuneClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("neptune") as client:  # (1)
    result = await client.add_role_to_db_cluster()  # (2)
```

1. client: [NeptuneClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeDBClusterEndpointsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("neptune") as client:  # (1)
    paginator = client.get_paginator("describe_db_cluster_endpoints")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [NeptuneClient](./client.md)
2. paginator: [DescribeDBClusterEndpointsPaginator](./paginators.md#describedbclusterendpointspaginator)
3. item: [:material-code-braces: DBClusterEndpointMessageTypeDef](./type_defs.md#dbclusterendpointmessagetypedef) 



```python
# DBInstanceAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("neptune") as client:  # (1)
    waiter = client.get_waiter("db_instance_available")  # (2)
    await waiter.wait()
```

1. client: [NeptuneClient](./client.md)
2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[neptune]`
or a standalone `types_aiobotocore_neptune` package, you have to explicitly specify
`client: NeptuneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# NeptuneClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_neptune.client import NeptuneClient
from types_aiobotocore_neptune.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_neptune.type_defs import AddRoleToDBClusterMessageTypeDef


session = get_session()

async with session.create_client("neptune") as client:
    client: NeptuneClient
    kwargs: AddRoleToDBClusterMessageTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.add_role_to_db_cluster(**kwargs)
```



```python
# DescribeDBClusterEndpointsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_neptune.client import NeptuneClient
from types_aiobotocore_neptune.paginator import DescribeDBClusterEndpointsPaginator
from types_aiobotocore_neptune.type_defs import DBClusterEndpointMessageTypeDef


session = get_session()

async with session.create_client("neptune") as client:
    client: NeptuneClient
    paginator: DescribeDBClusterEndpointsPaginator = client.get_paginator("describe_db_cluster_endpoints")
    async for item in paginator.paginate(...):
        item: DBClusterEndpointMessageTypeDef
        print(item)
```



```python
# DBInstanceAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_neptune.client import NeptuneClient
from types_aiobotocore_neptune.waiter import DBInstanceAvailableWaiter


session = get_session()

async with session.create_client("neptune") as client:
    client: NeptuneClient
    waiter: DBInstanceAvailableWaiter = client.get_waiter("db_instance_available")
    await waiter.wait()
```
