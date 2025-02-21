# Examples

> [Index](../README.md) > [OpsWorks](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[opsworks]` package installed.

Write your `OpsWorks` code as usual,
type checking and code completion should work out of the box.



```python
# OpsWorksClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opsworks") as client:  # (1)
    result = await client.assign_instance()  # (2)
```

1. client: [OpsWorksClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# DescribeEcsClustersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opsworks") as client:  # (1)
    paginator = client.get_paginator("describe_ecs_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OpsWorksClient](./client.md)
2. paginator: [DescribeEcsClustersPaginator](./paginators.md#describeecsclusterspaginator)
3. item: [:material-code-braces: DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef) 



```python
# AppExistsWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opsworks") as client:  # (1)
    waiter = client.get_waiter("app_exists")  # (2)
    await waiter.wait()
```

1. client: [OpsWorksClient](./client.md)
2. waiter: [AppExistsWaiter](./waiters.md#appexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[opsworks]`
or a standalone `types_aiobotocore_opsworks` package, you have to explicitly specify
`client: OpsWorksClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OpsWorksClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opsworks.client import OpsWorksClient
from types_aiobotocore_opsworks.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_opsworks.type_defs import AssignInstanceRequestTypeDef


session = get_session()

async with session.create_client("opsworks") as client:
    client: OpsWorksClient
    kwargs: AssignInstanceRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.assign_instance(**kwargs)
```



```python
# DescribeEcsClustersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opsworks.client import OpsWorksClient
from types_aiobotocore_opsworks.paginator import DescribeEcsClustersPaginator
from types_aiobotocore_opsworks.type_defs import DescribeEcsClustersResultTypeDef


session = get_session()

async with session.create_client("opsworks") as client:
    client: OpsWorksClient
    paginator: DescribeEcsClustersPaginator = client.get_paginator("describe_ecs_clusters")
    async for item in paginator.paginate(...):
        item: DescribeEcsClustersResultTypeDef
        print(item)
```



```python
# AppExistsWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opsworks.client import OpsWorksClient
from types_aiobotocore_opsworks.waiter import AppExistsWaiter


session = get_session()

async with session.create_client("opsworks") as client:
    client: OpsWorksClient
    waiter: AppExistsWaiter = client.get_waiter("app_exists")
    await waiter.wait()
```
