<a id="examples-for-aiobotocore-prometheusservice-module"></a>

# Examples for aiobotocore PrometheusService module

> [Index](../README.md) > [PrometheusService](./README.md) > Examples

- [Examples for aiobotocore PrometheusService module](#examples-for-aiobotocore-prometheusservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[amp]` package installed.

Write your `PrometheusService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PrometheusServiceClient
# and provides type checking and code completion
async with session.create_client("amp") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListRuleGroupsNamespacesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_rule_groups_namespaces")
    async for item in paginator.paginate(...):
        # item has type ListRuleGroupsNamespacesResponseTypeDef
        print(item)
    

    
    # waiter has type WorkspaceActiveWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("workspace_active")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[amp]` or a standalone `types_aiobotocore_amp`
package, you have to explicitly specify `client: PrometheusServiceClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_amp.client import PrometheusServiceClient
from types_aiobotocore_amp.type_defs import bool
from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator
from types_aiobotocore_amp.waiter import WorkspaceActiveWaiter
from types_aiobotocore_amp.literals import PaginatorName
from types_aiobotocore_amp.literals import WaiterName


session = get_session()

async with session.create_client("amp") as client:
    client: PrometheusServiceClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_rule_groups_namespaces"
    paginator: ListRuleGroupsNamespacesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListRuleGroupsNamespacesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "workspace_active"
    waiter: WorkspaceActiveWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
