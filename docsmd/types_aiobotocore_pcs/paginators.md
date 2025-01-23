# Paginators

> [Index](../README.md) > [ParallelComputingService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#parallelcomputingservice)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).

## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("pcs").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs/paginator/ListClusters.html#ParallelComputingService.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pcs.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("pcs") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef) 
## ListComputeNodeGroupsPaginator

Type annotations and code completion for `#!python session.create_client("pcs").get_paginator("list_compute_node_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs/paginator/ListComputeNodeGroups.html#ParallelComputingService.Paginator.ListComputeNodeGroups)

```python
# ListComputeNodeGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pcs.paginator import ListComputeNodeGroupsPaginator

session = get_session()
async with session.create_client("pcs") as client:  # (1)
    paginator: ListComputeNodeGroupsPaginator = client.get_paginator("list_compute_node_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListComputeNodeGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. paginator: [ListComputeNodeGroupsPaginator](./paginators.md#listcomputenodegroupspaginator)
3. item: [:material-code-braces: ListComputeNodeGroupsResponseTypeDef](./type_defs.md#listcomputenodegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComputeNodeGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListComputeNodeGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComputeNodeGroupsResponseTypeDef](./type_defs.md#listcomputenodegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListComputeNodeGroupsRequestPaginateTypeDef = {  # (1)
    "clusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComputeNodeGroupsRequestPaginateTypeDef](./type_defs.md#listcomputenodegroupsrequestpaginatetypedef) 
## ListQueuesPaginator

Type annotations and code completion for `#!python session.create_client("pcs").get_paginator("list_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs/paginator/ListQueues.html#ParallelComputingService.Paginator.ListQueues)

```python
# ListQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pcs.paginator import ListQueuesPaginator

session = get_session()
async with session.create_client("pcs") as client:  # (1)
    paginator: ListQueuesPaginator = client.get_paginator("list_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [ParallelComputingServiceClient](./client.md)
2. paginator: [ListQueuesPaginator](./paginators.md#listqueuespaginator)
3. item: [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    clusterIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListQueuesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQueuesRequestPaginateTypeDef = {  # (1)
    "clusterIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestPaginateTypeDef](./type_defs.md#listqueuesrequestpaginatetypedef) 
