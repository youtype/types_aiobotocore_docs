<a id="paginators-for-aiobotocore-emrcontainers-module"></a>

# Paginators for aiobotocore EMRContainers module

> [Index](../README.md) > [EMRContainers](./README.md) > Paginators

Auto-generated documentation for
[EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
type annotations stubs module
[types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

- [Paginators for aiobotocore EMRContainers module](#paginators-for-aiobotocore-emrcontainers-module)
  - [ListJobRunsPaginator](#listjobrunspaginator)
  - [ListManagedEndpointsPaginator](#listmanagedendpointspaginator)
  - [ListVirtualClustersPaginator](#listvirtualclusterspaginator)

<a id="listjobrunspaginator"></a>

## ListJobRunsPaginator

Type annotations for
`session.create_client("emr-containers").get_paginator("list_job_runs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListJobRunsPaginator

session = get_session()
async with session.create_client("emr-containers") as client:
    client: EMRContainersClient
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
```

Boto3 documentation:
[EMRContainers.Paginator.ListJobRuns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns)

Arguments for `ListJobRunsPaginator.paginate` method:

- `virtualClusterId`: `str` *(required)*
- `createdBefore`: `Union`\[`datetime`, `str`\]
- `createdAfter`: `Union`\[`datetime`, `str`\]
- `name`: `str`
- `states`: `Sequence`\[[JobRunStateType](./literals.md#jobrunstatetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobRunsPaginator.paginate` returns
`AsyncIterator`\[[ListJobRunsResponseTypeDef](./type_defs.md#listjobrunsresponsetypedef)\].

<a id="listmanagedendpointspaginator"></a>

## ListManagedEndpointsPaginator

Type annotations for
`session.create_client("emr-containers").get_paginator("list_managed_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListManagedEndpointsPaginator

session = get_session()
async with session.create_client("emr-containers") as client:
    client: EMRContainersClient
    paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")
```

Boto3 documentation:
[EMRContainers.Paginator.ListManagedEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints)

Arguments for `ListManagedEndpointsPaginator.paginate` method:

- `virtualClusterId`: `str` *(required)*
- `createdBefore`: `Union`\[`datetime`, `str`\]
- `createdAfter`: `Union`\[`datetime`, `str`\]
- `types`: `Sequence`\[`str`\]
- `states`: `Sequence`\[[EndpointStateType](./literals.md#endpointstatetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListManagedEndpointsPaginator.paginate` returns
`AsyncIterator`\[[ListManagedEndpointsResponseTypeDef](./type_defs.md#listmanagedendpointsresponsetypedef)\].

<a id="listvirtualclusterspaginator"></a>

## ListVirtualClustersPaginator

Type annotations for
`session.create_client("emr-containers").get_paginator("list_virtual_clusters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListVirtualClustersPaginator

session = get_session()
async with session.create_client("emr-containers") as client:
    client: EMRContainersClient
    paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")
```

Boto3 documentation:
[EMRContainers.Paginator.ListVirtualClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)

Arguments for `ListVirtualClustersPaginator.paginate` method:

- `containerProviderId`: `str`
- `containerProviderType`: `Literal['EKS']` (see
  [ContainerProviderTypeType](./literals.md#containerprovidertypetype))
- `createdAfter`: `Union`\[`datetime`, `str`\]
- `createdBefore`: `Union`\[`datetime`, `str`\]
- `states`:
  `Sequence`\[[VirtualClusterStateType](./literals.md#virtualclusterstatetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListVirtualClustersPaginator.paginate` returns
`AsyncIterator`\[[ListVirtualClustersResponseTypeDef](./type_defs.md#listvirtualclustersresponsetypedef)\].
