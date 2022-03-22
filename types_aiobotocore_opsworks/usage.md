<a id="examples-for-aiobotocore-opsworks-module"></a>

# Examples for aiobotocore OpsWorks module

> [Index](../README.md) > [OpsWorks](./README.md) > Examples

- [Examples for aiobotocore OpsWorks module](#examples-for-aiobotocore-opsworks-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[opsworks]` package installed.

Write your `OpsWorks` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type OpsWorksClient
# and provides type checking and code completion
async with session.create_client("opsworks") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.assign_instance()
    

    
    # paginator has type DescribeEcsClustersPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_ecs_clusters")
    async for item in paginator.paginate(...):
        # item has type DescribeEcsClustersResultTypeDef
        print(item)
    

    
    # waiter has type AppExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("app_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[opsworks]` or a standalone
`types_aiobotocore_opsworks` package, you have to explicitly specify
`client: OpsWorksClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_opsworks.client import OpsWorksClient
from types_aiobotocore_opsworks.type_defs import None
from types_aiobotocore_opsworks.paginator import DescribeEcsClustersPaginator
from types_aiobotocore_opsworks.waiter import AppExistsWaiter
from types_aiobotocore_opsworks.literals import PaginatorName
from types_aiobotocore_opsworks.literals import WaiterName


session = get_session()

async with session.create_client("opsworks") as client:
    client: OpsWorksClient

    
    result: None = client.assign_instance()
    

    
    paginator_name: PaginatorName = "describe_ecs_clusters"
    paginator: DescribeEcsClustersPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeEcsClustersResultTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "app_exists"
    waiter: AppExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
