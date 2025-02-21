# Paginators

> [Index](../README.md) > [NeptuneGraph](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#neptunegraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).

## ListExportTasksPaginator

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_paginator("list_export_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph/paginator/ListExportTasks.html#NeptuneGraph.Paginator.ListExportTasks)

```python
# ListExportTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.paginator import ListExportTasksPaginator

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    paginator: ListExportTasksPaginator = client.get_paginator("list_export_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListExportTasksOutputTypeDef
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListExportTasksPaginator](./paginators.md#listexporttaskspaginator)
3. item: [:material-code-braces: ListExportTasksOutputTypeDef](./type_defs.md#listexporttasksoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListExportTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    graphIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListExportTasksOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExportTasksOutputTypeDef](./type_defs.md#listexporttasksoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExportTasksInputPaginateTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExportTasksInputPaginateTypeDef](./type_defs.md#listexporttasksinputpaginatetypedef) 
## ListGraphSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_paginator("list_graph_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph/paginator/ListGraphSnapshots.html#NeptuneGraph.Paginator.ListGraphSnapshots)

```python
# ListGraphSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.paginator import ListGraphSnapshotsPaginator

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    paginator: ListGraphSnapshotsPaginator = client.get_paginator("list_graph_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: ListGraphSnapshotsOutputTypeDef
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListGraphSnapshotsPaginator](./paginators.md#listgraphsnapshotspaginator)
3. item: [:material-code-braces: ListGraphSnapshotsOutputTypeDef](./type_defs.md#listgraphsnapshotsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGraphSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    graphIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGraphSnapshotsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGraphSnapshotsOutputTypeDef](./type_defs.md#listgraphsnapshotsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGraphSnapshotsInputPaginateTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGraphSnapshotsInputPaginateTypeDef](./type_defs.md#listgraphsnapshotsinputpaginatetypedef) 
## ListGraphsPaginator

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_paginator("list_graphs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph/paginator/ListGraphs.html#NeptuneGraph.Paginator.ListGraphs)

```python
# ListGraphsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.paginator import ListGraphsPaginator

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    paginator: ListGraphsPaginator = client.get_paginator("list_graphs")  # (2)
    async for item in paginator.paginate(...):
        item: ListGraphsOutputTypeDef
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListGraphsPaginator](./paginators.md#listgraphspaginator)
3. item: [:material-code-braces: ListGraphsOutputTypeDef](./type_defs.md#listgraphsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGraphsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGraphsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGraphsOutputTypeDef](./type_defs.md#listgraphsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGraphsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGraphsInputPaginateTypeDef](./type_defs.md#listgraphsinputpaginatetypedef) 
## ListImportTasksPaginator

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_paginator("list_import_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph/paginator/ListImportTasks.html#NeptuneGraph.Paginator.ListImportTasks)

```python
# ListImportTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.paginator import ListImportTasksPaginator

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    paginator: ListImportTasksPaginator = client.get_paginator("list_import_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportTasksOutputTypeDef
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListImportTasksPaginator](./paginators.md#listimporttaskspaginator)
3. item: [:material-code-braces: ListImportTasksOutputTypeDef](./type_defs.md#listimporttasksoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListImportTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListImportTasksOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListImportTasksOutputTypeDef](./type_defs.md#listimporttasksoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImportTasksInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportTasksInputPaginateTypeDef](./type_defs.md#listimporttasksinputpaginatetypedef) 
## ListPrivateGraphEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("neptune-graph").get_paginator("list_private_graph_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph/paginator/ListPrivateGraphEndpoints.html#NeptuneGraph.Paginator.ListPrivateGraphEndpoints)

```python
# ListPrivateGraphEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.paginator import ListPrivateGraphEndpointsPaginator

session = get_session()
async with session.create_client("neptune-graph") as client:  # (1)
    paginator: ListPrivateGraphEndpointsPaginator = client.get_paginator("list_private_graph_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrivateGraphEndpointsOutputTypeDef
        print(item)  # (3)
```

1. client: [NeptuneGraphClient](./client.md)
2. paginator: [ListPrivateGraphEndpointsPaginator](./paginators.md#listprivategraphendpointspaginator)
3. item: [:material-code-braces: ListPrivateGraphEndpointsOutputTypeDef](./type_defs.md#listprivategraphendpointsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPrivateGraphEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    graphIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPrivateGraphEndpointsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPrivateGraphEndpointsOutputTypeDef](./type_defs.md#listprivategraphendpointsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPrivateGraphEndpointsInputPaginateTypeDef = {  # (1)
    "graphIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrivateGraphEndpointsInputPaginateTypeDef](./type_defs.md#listprivategraphendpointsinputpaginatetypedef) 
