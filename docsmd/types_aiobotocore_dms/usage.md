# Examples

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#databasemigrationservice)
    type annotations stubs module [types-aiobotocore-dms](https://pypi.org/project/types-aiobotocore-dms/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[dms]` package installed.

Write your `DatabaseMigrationService` code as usual,
type checking and code completion should work out of the box.



```python
# DatabaseMigrationServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dms") as client:  # (1)
    result = await client.apply_pending_maintenance_action()  # (2)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. result: [:material-code-braces: ApplyPendingMaintenanceActionResponseTypeDef](./type_defs.md#applypendingmaintenanceactionresponsetypedef) 



```python
# DescribeCertificatesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dms") as client:  # (1)
    paginator = client.get_paginator("describe_certificates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
3. item: [:material-code-braces: DescribeCertificatesResponseTypeDef](./type_defs.md#describecertificatesresponsetypedef) 



```python
# EndpointDeletedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("dms") as client:  # (1)
    waiter = client.get_waiter("endpoint_deleted")  # (2)
    await waiter.wait()
```

1. client: [DatabaseMigrationServiceClient](./client.md)
2. waiter: [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[dms]`
or a standalone `types_aiobotocore_dms` package, you have to explicitly specify
`client: DatabaseMigrationServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DatabaseMigrationServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dms.client import DatabaseMigrationServiceClient
from types_aiobotocore_dms.type_defs import ApplyPendingMaintenanceActionResponseTypeDef
from types_aiobotocore_dms.type_defs import ApplyPendingMaintenanceActionMessageTypeDef


session = get_session()

async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    kwargs: ApplyPendingMaintenanceActionMessageTypeDef = {...}
    result: ApplyPendingMaintenanceActionResponseTypeDef = await client.apply_pending_maintenance_action(**kwargs)
```



```python
# DescribeCertificatesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dms.client import DatabaseMigrationServiceClient
from types_aiobotocore_dms.paginator import DescribeCertificatesPaginator
from types_aiobotocore_dms.type_defs import DescribeCertificatesResponseTypeDef


session = get_session()

async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")
    async for item in paginator.paginate(...):
        item: DescribeCertificatesResponseTypeDef
        print(item)
```



```python
# EndpointDeletedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_dms.client import DatabaseMigrationServiceClient
from types_aiobotocore_dms.waiter import EndpointDeletedWaiter


session = get_session()

async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient
    waiter: EndpointDeletedWaiter = client.get_waiter("endpoint_deleted")
    await waiter.wait()
```
