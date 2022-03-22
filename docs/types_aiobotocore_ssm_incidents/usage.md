<a id="examples-for-aiobotocore-ssmincidents-module"></a>

# Examples for aiobotocore SSMIncidents module

> [Index](../README.md) > [SSMIncidents](./README.md) > Examples

- [Examples for aiobotocore SSMIncidents module](#examples-for-aiobotocore-ssmincidents-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ssm-incidents]` package installed.

Write your `SSMIncidents` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SSMIncidentsClient
# and provides type checking and code completion
async with session.create_client("ssm-incidents") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetResourcePoliciesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_resource_policies")
    async for item in paginator.paginate(...):
        # item has type GetResourcePoliciesOutputTypeDef
        print(item)
    

    
    # waiter has type WaitForReplicationSetActiveWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("wait_for_replication_set_active")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ssm-incidents]` or a standalone
`types_aiobotocore_ssm_incidents` package, you have to explicitly specify
`client: SSMIncidentsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient
from types_aiobotocore_ssm_incidents.type_defs import bool
from types_aiobotocore_ssm_incidents.paginator import GetResourcePoliciesPaginator
from types_aiobotocore_ssm_incidents.waiter import WaitForReplicationSetActiveWaiter
from types_aiobotocore_ssm_incidents.literals import PaginatorName
from types_aiobotocore_ssm_incidents.literals import WaiterName


session = get_session()

async with session.create_client("ssm-incidents") as client:
    client: SSMIncidentsClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_resource_policies"
    paginator: GetResourcePoliciesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "wait_for_replication_set_active"
    waiter: WaitForReplicationSetActiveWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
