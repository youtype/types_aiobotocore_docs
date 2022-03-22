<a id="examples-for-aiobotocore-opsworkscm-module"></a>

# Examples for aiobotocore OpsWorksCM module

> [Index](../README.md) > [OpsWorksCM](./README.md) > Examples

- [Examples for aiobotocore OpsWorksCM module](#examples-for-aiobotocore-opsworkscm-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[opsworkscm]` package installed.

Write your `OpsWorksCM` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type OpsWorksCMClient
# and provides type checking and code completion
async with session.create_client("opsworkscm") as client:
    
    # result has type AssociateNodeResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_node()
    

    
    # paginator has type DescribeBackupsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_backups")
    async for item in paginator.paginate(...):
        # item has type DescribeBackupsResponseTypeDef
        print(item)
    

    
    # waiter has type NodeAssociatedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("node_associated")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[opsworkscm]` or a standalone
`types_aiobotocore_opsworkscm` package, you have to explicitly specify
`client: OpsWorksCMClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.client import OpsWorksCMClient
from types_aiobotocore_opsworkscm.type_defs import AssociateNodeResponseTypeDef
from types_aiobotocore_opsworkscm.paginator import DescribeBackupsPaginator
from types_aiobotocore_opsworkscm.waiter import NodeAssociatedWaiter
from types_aiobotocore_opsworkscm.literals import PaginatorName
from types_aiobotocore_opsworkscm.literals import WaiterName


session = get_session()

async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient

    
    result: AssociateNodeResponseTypeDef = client.associate_node()
    

    
    paginator_name: PaginatorName = "describe_backups"
    paginator: DescribeBackupsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "node_associated"
    waiter: NodeAssociatedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
