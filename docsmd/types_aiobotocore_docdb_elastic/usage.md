# Examples

> [Index](../README.md) > [DocDBElastic](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#docdbelastic)
    type annotations stubs module [types-aiobotocore-docdb-elastic](https://pypi.org/project/types-aiobotocore-docdb-elastic/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[docdb-elastic]` package installed.

Write your `DocDBElastic` code as usual,
type checking and code completion should work out of the box.



```python
# DocDBElasticClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("docdb-elastic") as client:  # (1)
    result = await client.apply_pending_maintenance_action()  # (2)
```

1. client: [DocDBElasticClient](./client.md)
2. result: [:material-code-braces: ApplyPendingMaintenanceActionOutputTypeDef](./type_defs.md#applypendingmaintenanceactionoutputtypedef) 



```python
# ListClusterSnapshotsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("docdb-elastic") as client:  # (1)
    paginator = client.get_paginator("list_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DocDBElasticClient](./client.md)
2. paginator: [ListClusterSnapshotsPaginator](./paginators.md#listclustersnapshotspaginator)
3. item: [:material-code-braces: ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[docdb-elastic]`
or a standalone `types_aiobotocore_docdb_elastic` package, you have to explicitly specify
`client: DocDBElasticClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DocDBElasticClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_docdb_elastic.client import DocDBElasticClient
from types_aiobotocore_docdb_elastic.type_defs import ApplyPendingMaintenanceActionOutputTypeDef
from types_aiobotocore_docdb_elastic.type_defs import ApplyPendingMaintenanceActionInputTypeDef


session = get_session()

async with session.create_client("docdb-elastic") as client:
    client: DocDBElasticClient
    kwargs: ApplyPendingMaintenanceActionInputTypeDef = {...}
    result: ApplyPendingMaintenanceActionOutputTypeDef = await client.apply_pending_maintenance_action(**kwargs)
```



```python
# ListClusterSnapshotsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_docdb_elastic.client import DocDBElasticClient
from types_aiobotocore_docdb_elastic.paginator import ListClusterSnapshotsPaginator
from types_aiobotocore_docdb_elastic.type_defs import ListClusterSnapshotsOutputTypeDef


session = get_session()

async with session.create_client("docdb-elastic") as client:
    client: DocDBElasticClient
    paginator: ListClusterSnapshotsPaginator = client.get_paginator("list_cluster_snapshots")
    async for item in paginator.paginate(...):
        item: ListClusterSnapshotsOutputTypeDef
        print(item)
```


