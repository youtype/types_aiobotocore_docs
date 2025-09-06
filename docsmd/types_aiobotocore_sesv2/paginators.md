# Paginators

> [Index](../README.md) > [SESV2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#sesv2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## ListMultiRegionEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("sesv2").get_paginator("list_multi_region_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/paginator/ListMultiRegionEndpoints.html#SESV2.Paginator.ListMultiRegionEndpoints)

```python
# ListMultiRegionEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sesv2.paginator import ListMultiRegionEndpointsPaginator

session = get_session()
async with session.create_client("sesv2") as client:  # (1)
    paginator: ListMultiRegionEndpointsPaginator = client.get_paginator("list_multi_region_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListMultiRegionEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListMultiRegionEndpointsPaginator](./paginators.md#listmultiregionendpointspaginator)
3. item: `AioPageIterator[ListMultiRegionEndpointsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMultiRegionEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMultiRegionEndpointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMultiRegionEndpointsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMultiRegionEndpointsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultiRegionEndpointsRequestPaginateTypeDef](./type_defs.md#listmultiregionendpointsrequestpaginatetypedef)
## ListReputationEntitiesPaginator

Type annotations and code completion for `#!python session.create_client("sesv2").get_paginator("list_reputation_entities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/paginator/ListReputationEntities.html#SESV2.Paginator.ListReputationEntities)

```python
# ListReputationEntitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sesv2.paginator import ListReputationEntitiesPaginator

session = get_session()
async with session.create_client("sesv2") as client:  # (1)
    paginator: ListReputationEntitiesPaginator = client.get_paginator("list_reputation_entities")  # (2)
    async for item in paginator.paginate(...):
        item: ListReputationEntitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListReputationEntitiesPaginator](./paginators.md#listreputationentitiespaginator)
3. item: `AioPageIterator[ListReputationEntitiesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReputationEntitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: Mapping[ReputationEntityFilterKeyType, str] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListReputationEntitiesResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[ReputationEntityFilterKeyType, str]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListReputationEntitiesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReputationEntitiesRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReputationEntitiesRequestPaginateTypeDef](./type_defs.md#listreputationentitiesrequestpaginatetypedef)
## ListResourceTenantsPaginator

Type annotations and code completion for `#!python session.create_client("sesv2").get_paginator("list_resource_tenants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/paginator/ListResourceTenants.html#SESV2.Paginator.ListResourceTenants)

```python
# ListResourceTenantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sesv2.paginator import ListResourceTenantsPaginator

session = get_session()
async with session.create_client("sesv2") as client:  # (1)
    paginator: ListResourceTenantsPaginator = client.get_paginator("list_resource_tenants")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceTenantsResponseTypeDef
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListResourceTenantsPaginator](./paginators.md#listresourcetenantspaginator)
3. item: `AioPageIterator[ListResourceTenantsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResourceTenantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListResourceTenantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListResourceTenantsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceTenantsRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceTenantsRequestPaginateTypeDef](./type_defs.md#listresourcetenantsrequestpaginatetypedef)
## ListTenantResourcesPaginator

Type annotations and code completion for `#!python session.create_client("sesv2").get_paginator("list_tenant_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/paginator/ListTenantResources.html#SESV2.Paginator.ListTenantResources)

```python
# ListTenantResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sesv2.paginator import ListTenantResourcesPaginator

session = get_session()
async with session.create_client("sesv2") as client:  # (1)
    paginator: ListTenantResourcesPaginator = client.get_paginator("list_tenant_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListTenantResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListTenantResourcesPaginator](./paginators.md#listtenantresourcespaginator)
3. item: `AioPageIterator[ListTenantResourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTenantResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TenantName: str,
    Filter: Mapping[ListTenantResourcesFilterKeyType, str] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListTenantResourcesResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[Literal['RESOURCE_TYPE'], str]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListTenantResourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTenantResourcesRequestPaginateTypeDef = {  # (1)
    "TenantName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTenantResourcesRequestPaginateTypeDef](./type_defs.md#listtenantresourcesrequestpaginatetypedef)
## ListTenantsPaginator

Type annotations and code completion for `#!python session.create_client("sesv2").get_paginator("list_tenants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2/paginator/ListTenants.html#SESV2.Paginator.ListTenants)

```python
# ListTenantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sesv2.paginator import ListTenantsPaginator

session = get_session()
async with session.create_client("sesv2") as client:  # (1)
    paginator: ListTenantsPaginator = client.get_paginator("list_tenants")  # (2)
    async for item in paginator.paginate(...):
        item: ListTenantsResponseTypeDef
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListTenantsPaginator](./paginators.md#listtenantspaginator)
3. item: `AioPageIterator[ListTenantsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTenantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTenantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTenantsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTenantsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTenantsRequestPaginateTypeDef](./type_defs.md#listtenantsrequestpaginatetypedef)
