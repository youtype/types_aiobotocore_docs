# Paginators

> [Index](../README.md) > [EMRContainers](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#emrcontainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## ListJobRunsPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_job_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers/paginator/ListJobRuns.html#EMRContainers.Paginator.ListJobRuns)

```python
# ListJobRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListJobRunsPaginator

session = get_session()
async with session.create_client("emr-containers") as client:  # (1)
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobRunsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
3. item: [:material-code-braces: ListJobRunsResponsePaginatorTypeDef](./type_defs.md#listjobrunsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListJobRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    virtualClusterId: str,
    createdBefore: TimestampTypeDef = ...,
    createdAfter: TimestampTypeDef = ...,
    name: str = ...,
    states: Sequence[JobRunStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListJobRunsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListJobRunsResponsePaginatorTypeDef](./type_defs.md#listjobrunsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobRunsRequestPaginateTypeDef = {  # (1)
    "virtualClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobRunsRequestPaginateTypeDef](./type_defs.md#listjobrunsrequestpaginatetypedef) 
## ListJobTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_job_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers/paginator/ListJobTemplates.html#EMRContainers.Paginator.ListJobTemplates)

```python
# ListJobTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListJobTemplatesPaginator

session = get_session()
async with session.create_client("emr-containers") as client:  # (1)
    paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobTemplatesResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListJobTemplatesPaginator](./paginators.md#listjobtemplatespaginator)
3. item: [:material-code-braces: ListJobTemplatesResponsePaginatorTypeDef](./type_defs.md#listjobtemplatesresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListJobTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    createdAfter: TimestampTypeDef = ...,
    createdBefore: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListJobTemplatesResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobTemplatesResponsePaginatorTypeDef](./type_defs.md#listjobtemplatesresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobTemplatesRequestPaginateTypeDef = {  # (1)
    "createdAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobTemplatesRequestPaginateTypeDef](./type_defs.md#listjobtemplatesrequestpaginatetypedef) 
## ListManagedEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_managed_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers/paginator/ListManagedEndpoints.html#EMRContainers.Paginator.ListManagedEndpoints)

```python
# ListManagedEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListManagedEndpointsPaginator

session = get_session()
async with session.create_client("emr-containers") as client:  # (1)
    paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedEndpointsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListManagedEndpointsPaginator](./paginators.md#listmanagedendpointspaginator)
3. item: [:material-code-braces: ListManagedEndpointsResponsePaginatorTypeDef](./type_defs.md#listmanagedendpointsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    virtualClusterId: str,
    createdBefore: TimestampTypeDef = ...,
    createdAfter: TimestampTypeDef = ...,
    types: Sequence[str] = ...,
    states: Sequence[EndpointStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListManagedEndpointsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListManagedEndpointsResponsePaginatorTypeDef](./type_defs.md#listmanagedendpointsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedEndpointsRequestPaginateTypeDef = {  # (1)
    "virtualClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedEndpointsRequestPaginateTypeDef](./type_defs.md#listmanagedendpointsrequestpaginatetypedef) 
## ListSecurityConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_security_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers/paginator/ListSecurityConfigurations.html#EMRContainers.Paginator.ListSecurityConfigurations)

```python
# ListSecurityConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.paginator import ListSecurityConfigurationsPaginator

session = get_session()
async with session.create_client("emr-containers") as client:  # (1)
    paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListSecurityConfigurationsPaginator](./paginators.md#listsecurityconfigurationspaginator)
3. item: [:material-code-braces: ListSecurityConfigurationsResponseTypeDef](./type_defs.md#listsecurityconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecurityConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    createdAfter: TimestampTypeDef = ...,
    createdBefore: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSecurityConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSecurityConfigurationsResponseTypeDef](./type_defs.md#listsecurityconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityConfigurationsRequestPaginateTypeDef = {  # (1)
    "createdAfter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityConfigurationsRequestPaginateTypeDef](./type_defs.md#listsecurityconfigurationsrequestpaginatetypedef) 
## ListVirtualClustersPaginator

Type annotations and code completion for `#!python session.create_client("emr-containers").get_paginator("list_virtual_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers/paginator/ListVirtualClusters.html#EMRContainers.Paginator.ListVirtualClusters)

```python
# ListVirtualClustersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    containerProviderId: str = ...,
    containerProviderType: ContainerProviderTypeType = ...,  # (1)
    createdAfter: TimestampTypeDef = ...,
    createdBefore: TimestampTypeDef = ...,
    states: Sequence[VirtualClusterStateType] = ...,  # (2)
    eksAccessEntryIntegrated: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListVirtualClustersResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ContainerProviderTypeType](./literals.md#containerprovidertypetype) 
2. See [:material-code-brackets: VirtualClusterStateType](./literals.md#virtualclusterstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListVirtualClustersResponseTypeDef](./type_defs.md#listvirtualclustersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVirtualClustersRequestPaginateTypeDef = {  # (1)
    "containerProviderId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualClustersRequestPaginateTypeDef](./type_defs.md#listvirtualclustersrequestpaginatetypedef) 
