# Examples

> [Index](../README.md) > [OpsWorksCM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#opsworkscm)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[opsworkscm]` package installed.

Write your `OpsWorksCM` code as usual,
type checking and code completion should work out of the box.



```python
# OpsWorksCMClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opsworkscm") as client:  # (1)
    result = await client.associate_node()  # (2)
```

1. client: [OpsWorksCMClient](./client.md)
2. result: [:material-code-braces: AssociateNodeResponseTypeDef](./type_defs.md#associatenoderesponsetypedef) 



```python
# DescribeBackupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opsworkscm") as client:  # (1)
    paginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OpsWorksCMClient](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 



```python
# NodeAssociatedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("opsworkscm") as client:  # (1)
    waiter = client.get_waiter("node_associated")  # (2)
    await waiter.wait()
```

1. client: [OpsWorksCMClient](./client.md)
2. waiter: [NodeAssociatedWaiter](./waiters.md#nodeassociatedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[opsworkscm]`
or a standalone `types_aiobotocore_opsworkscm` package, you have to explicitly specify
`client: OpsWorksCMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OpsWorksCMClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.client import OpsWorksCMClient
from types_aiobotocore_opsworkscm.type_defs import AssociateNodeResponseTypeDef
from types_aiobotocore_opsworkscm.type_defs import AssociateNodeRequestTypeDef


session = get_session()

async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
    kwargs: AssociateNodeRequestTypeDef = {...}
    result: AssociateNodeResponseTypeDef = await client.associate_node(**kwargs)
```



```python
# DescribeBackupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.client import OpsWorksCMClient
from types_aiobotocore_opsworkscm.paginator import DescribeBackupsPaginator
from types_aiobotocore_opsworkscm.type_defs import DescribeBackupsResponseTypeDef


session = get_session()

async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponseTypeDef
        print(item)
```



```python
# NodeAssociatedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.client import OpsWorksCMClient
from types_aiobotocore_opsworkscm.waiter import NodeAssociatedWaiter


session = get_session()

async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
    waiter: NodeAssociatedWaiter = client.get_waiter("node_associated")
    await waiter.wait()
```
