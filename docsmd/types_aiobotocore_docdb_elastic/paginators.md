# Paginators

> [Index](../README.md) > [DocDBElastic](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#docdbelastic)
    type annotations stubs module [types-aiobotocore-docdb-elastic](https://pypi.org/project/types-aiobotocore-docdb-elastic/).

## ListClusterSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("docdb-elastic").get_paginator("list_cluster_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic/paginator/ListClusterSnapshots.html#DocDBElastic.Paginator.ListClusterSnapshots)

```python
# ListClusterSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_docdb_elastic.paginator import ListClusterSnapshotsPaginator

session = get_session()
async with session.create_client("docdb-elastic") as client:  # (1)
    paginator: ListClusterSnapshotsPaginator = client.get_paginator("list_cluster_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: ListClusterSnapshotsOutputTypeDef
        print(item)  # (3)
```

1. client: [DocDBElasticClient](./client.md)
2. paginator: [ListClusterSnapshotsPaginator](./paginators.md#listclustersnapshotspaginator)
3. item: [:material-code-braces: ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListClusterSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterArn: str = ...,
    snapshotType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClusterSnapshotsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClusterSnapshotsInputPaginateTypeDef = {  # (1)
    "clusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClusterSnapshotsInputPaginateTypeDef](./type_defs.md#listclustersnapshotsinputpaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("docdb-elastic").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic/paginator/ListClusters.html#DocDBElastic.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_docdb_elastic.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("docdb-elastic") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersOutputTypeDef
        print(item)  # (3)
```

1. client: [DocDBElasticClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClustersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersInputPaginateTypeDef](./type_defs.md#listclustersinputpaginatetypedef) 
## ListPendingMaintenanceActionsPaginator

Type annotations and code completion for `#!python session.create_client("docdb-elastic").get_paginator("list_pending_maintenance_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic/paginator/ListPendingMaintenanceActions.html#DocDBElastic.Paginator.ListPendingMaintenanceActions)

```python
# ListPendingMaintenanceActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_docdb_elastic.paginator import ListPendingMaintenanceActionsPaginator

session = get_session()
async with session.create_client("docdb-elastic") as client:  # (1)
    paginator: ListPendingMaintenanceActionsPaginator = client.get_paginator("list_pending_maintenance_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPendingMaintenanceActionsOutputTypeDef
        print(item)  # (3)
```

1. client: [DocDBElasticClient](./client.md)
2. paginator: [ListPendingMaintenanceActionsPaginator](./paginators.md#listpendingmaintenanceactionspaginator)
3. item: [:material-code-braces: ListPendingMaintenanceActionsOutputTypeDef](./type_defs.md#listpendingmaintenanceactionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPendingMaintenanceActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPendingMaintenanceActionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPendingMaintenanceActionsOutputTypeDef](./type_defs.md#listpendingmaintenanceactionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPendingMaintenanceActionsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPendingMaintenanceActionsInputPaginateTypeDef](./type_defs.md#listpendingmaintenanceactionsinputpaginatetypedef) 
