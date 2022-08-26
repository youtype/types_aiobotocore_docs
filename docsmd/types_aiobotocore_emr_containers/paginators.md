# Paginators

> [Index](../README.md) > [EMRContainers](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## ListJobRunsPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListJobRunsPaginator

session = get_session()
async with session.create_client("emr-containers") as client:  # (1)
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
3. item: [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobRunsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    virtualClusterId: str,
    createdBefore: Union[datetime, str] = ...,
    createdAfter: Union[datetime, str] = ...,
    name: str = ...,
    states: Sequence[JobRunStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListJobRunsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobRunsRequestListJobRunsPaginateTypeDef = {  # (1)
    "virtualClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestListJobRunsPaginateTypeDef](./type_defs.md#listjobrunsrequestlistjobrunspaginatetypedef) 
## ListManagedEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_managed_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListManagedEndpointsPaginator

session = get_session()
async with session.create_client("emr-containers") as client:  # (1)
    paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListManagedEndpointsPaginator](./paginators.md#listmanagedendpointspaginator)
3. item: [:material-code-braces: ListManagedEndpointsResponseTypeDef](./type_defs.md#listmanagedendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    virtualClusterId: str,
    createdBefore: Union[datetime, str] = ...,
    createdAfter: Union[datetime, str] = ...,
    types: Sequence[str] = ...,
    states: Sequence[EndpointStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListManagedEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListManagedEndpointsResponseTypeDef](./type_defs.md#listmanagedendpointsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = {  # (1)
    "virtualClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef](./type_defs.md#listmanagedendpointsrequestlistmanagedendpointspaginatetypedef) 
## ListVirtualClustersPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_virtual_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListVirtualClustersPaginator

session = get_session()
async with session.create_client("emr-containers") as client:  # (1)
    paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListVirtualClustersPaginator](./paginators.md#listvirtualclusterspaginator)
3. item: [:material-code-braces: ListVirtualClustersResponseTypeDef](./type_defs.md#listvirtualclustersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualClustersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    containerProviderId: str = ...,
    containerProviderType: ContainerProviderTypeType = ...,  # (1)
    createdAfter: Union[datetime, str] = ...,
    createdBefore: Union[datetime, str] = ...,
    states: Sequence[VirtualClusterStateType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListVirtualClustersResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ContainerProviderTypeType](./literals.md#containerprovidertypetype) 
2. See [:material-code-brackets: VirtualClusterStateType](./literals.md#virtualclusterstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListVirtualClustersResponseTypeDef](./type_defs.md#listvirtualclustersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = {  # (1)
    "containerProviderId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualClustersRequestListVirtualClustersPaginateTypeDef](./type_defs.md#listvirtualclustersrequestlistvirtualclusterspaginatetypedef) 
