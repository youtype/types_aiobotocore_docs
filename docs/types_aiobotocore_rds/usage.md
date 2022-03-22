<a id="examples-for-aiobotocore-rds-module"></a>

# Examples for aiobotocore RDS module

> [Index](../README.md) > [RDS](./README.md) > Examples

- [Examples for aiobotocore RDS module](#examples-for-aiobotocore-rds-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[rds]` package installed.

Write your `RDS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RDSClient
# and provides type checking and code completion
async with session.create_client("rds") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_role_to_db_cluster()
    

    
    # paginator has type DescribeCertificatesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_certificates")
    async for item in paginator.paginate(...):
        # item has type CertificateMessageTypeDef
        print(item)
    

    
    # waiter has type DBClusterSnapshotAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("db_cluster_snapshot_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[rds]` or a standalone `types_aiobotocore_rds`
package, you have to explicitly specify `client: RDSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_rds.client import RDSClient
from types_aiobotocore_rds.type_defs import None
from types_aiobotocore_rds.paginator import DescribeCertificatesPaginator
from types_aiobotocore_rds.waiter import DBClusterSnapshotAvailableWaiter
from types_aiobotocore_rds.literals import PaginatorName
from types_aiobotocore_rds.literals import WaiterName


session = get_session()

async with session.create_client("rds") as client:
    client: RDSClient

    
    result: None = client.add_role_to_db_cluster()
    

    
    paginator_name: PaginatorName = "describe_certificates"
    paginator: DescribeCertificatesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: CertificateMessageTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "db_cluster_snapshot_available"
    waiter: DBClusterSnapshotAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
