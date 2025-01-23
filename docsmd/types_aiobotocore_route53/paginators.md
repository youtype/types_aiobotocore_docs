# Paginators

> [Index](../README.md) > [Route53](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#route53)
    type annotations stubs module [types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

## ListCidrBlocksPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_cidr_blocks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListCidrBlocks.html#Route53.Paginator.ListCidrBlocks)

```python
# ListCidrBlocksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListCidrBlocksPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListCidrBlocksPaginator = client.get_paginator("list_cidr_blocks")  # (2)
    async for item in paginator.paginate(...):
        item: ListCidrBlocksResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListCidrBlocksPaginator](./paginators.md#listcidrblockspaginator)
3. item: [:material-code-braces: ListCidrBlocksResponseTypeDef](./type_defs.md#listcidrblocksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCidrBlocksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CollectionId: str,
    LocationName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCidrBlocksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCidrBlocksResponseTypeDef](./type_defs.md#listcidrblocksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCidrBlocksRequestPaginateTypeDef = {  # (1)
    "CollectionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCidrBlocksRequestPaginateTypeDef](./type_defs.md#listcidrblocksrequestpaginatetypedef) 
## ListCidrCollectionsPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_cidr_collections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListCidrCollections.html#Route53.Paginator.ListCidrCollections)

```python
# ListCidrCollectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListCidrCollectionsPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListCidrCollectionsPaginator = client.get_paginator("list_cidr_collections")  # (2)
    async for item in paginator.paginate(...):
        item: ListCidrCollectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListCidrCollectionsPaginator](./paginators.md#listcidrcollectionspaginator)
3. item: [:material-code-braces: ListCidrCollectionsResponseTypeDef](./type_defs.md#listcidrcollectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCidrCollectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCidrCollectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCidrCollectionsResponseTypeDef](./type_defs.md#listcidrcollectionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCidrCollectionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCidrCollectionsRequestPaginateTypeDef](./type_defs.md#listcidrcollectionsrequestpaginatetypedef) 
## ListCidrLocationsPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_cidr_locations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListCidrLocations.html#Route53.Paginator.ListCidrLocations)

```python
# ListCidrLocationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListCidrLocationsPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListCidrLocationsPaginator = client.get_paginator("list_cidr_locations")  # (2)
    async for item in paginator.paginate(...):
        item: ListCidrLocationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListCidrLocationsPaginator](./paginators.md#listcidrlocationspaginator)
3. item: [:material-code-braces: ListCidrLocationsResponseTypeDef](./type_defs.md#listcidrlocationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCidrLocationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CollectionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCidrLocationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCidrLocationsResponseTypeDef](./type_defs.md#listcidrlocationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCidrLocationsRequestPaginateTypeDef = {  # (1)
    "CollectionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCidrLocationsRequestPaginateTypeDef](./type_defs.md#listcidrlocationsrequestpaginatetypedef) 
## ListHealthChecksPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_health_checks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListHealthChecks.html#Route53.Paginator.ListHealthChecks)

```python
# ListHealthChecksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListHealthChecksPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListHealthChecksPaginator = client.get_paginator("list_health_checks")  # (2)
    async for item in paginator.paginate(...):
        item: ListHealthChecksResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListHealthChecksPaginator](./paginators.md#listhealthcheckspaginator)
3. item: [:material-code-braces: ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHealthChecksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListHealthChecksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHealthChecksResponseTypeDef](./type_defs.md#listhealthchecksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHealthChecksRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHealthChecksRequestPaginateTypeDef](./type_defs.md#listhealthchecksrequestpaginatetypedef) 
## ListHostedZonesPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_hosted_zones")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListHostedZones.html#Route53.Paginator.ListHostedZones)

```python
# ListHostedZonesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListHostedZonesPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListHostedZonesPaginator = client.get_paginator("list_hosted_zones")  # (2)
    async for item in paginator.paginate(...):
        item: ListHostedZonesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListHostedZonesPaginator](./paginators.md#listhostedzonespaginator)
3. item: [:material-code-braces: ListHostedZonesResponseTypeDef](./type_defs.md#listhostedzonesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHostedZonesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DelegationSetId: str = ...,
    HostedZoneType: HostedZoneTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListHostedZonesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: HostedZoneTypeType](./literals.md#hostedzonetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHostedZonesResponseTypeDef](./type_defs.md#listhostedzonesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHostedZonesRequestPaginateTypeDef = {  # (1)
    "DelegationSetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHostedZonesRequestPaginateTypeDef](./type_defs.md#listhostedzonesrequestpaginatetypedef) 
## ListQueryLoggingConfigsPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_query_logging_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListQueryLoggingConfigs.html#Route53.Paginator.ListQueryLoggingConfigs)

```python
# ListQueryLoggingConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListQueryLoggingConfigsPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListQueryLoggingConfigsPaginator = client.get_paginator("list_query_logging_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueryLoggingConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListQueryLoggingConfigsPaginator](./paginators.md#listqueryloggingconfigspaginator)
3. item: [:material-code-braces: ListQueryLoggingConfigsResponseTypeDef](./type_defs.md#listqueryloggingconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQueryLoggingConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HostedZoneId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListQueryLoggingConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQueryLoggingConfigsResponseTypeDef](./type_defs.md#listqueryloggingconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQueryLoggingConfigsRequestPaginateTypeDef = {  # (1)
    "HostedZoneId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueryLoggingConfigsRequestPaginateTypeDef](./type_defs.md#listqueryloggingconfigsrequestpaginatetypedef) 
## ListResourceRecordSetsPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_resource_record_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListResourceRecordSets.html#Route53.Paginator.ListResourceRecordSets)

```python
# ListResourceRecordSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListResourceRecordSetsPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListResourceRecordSetsPaginator = client.get_paginator("list_resource_record_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceRecordSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListResourceRecordSetsPaginator](./paginators.md#listresourcerecordsetspaginator)
3. item: [:material-code-braces: ListResourceRecordSetsResponseTypeDef](./type_defs.md#listresourcerecordsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceRecordSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HostedZoneId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResourceRecordSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceRecordSetsResponseTypeDef](./type_defs.md#listresourcerecordsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceRecordSetsRequestPaginateTypeDef = {  # (1)
    "HostedZoneId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceRecordSetsRequestPaginateTypeDef](./type_defs.md#listresourcerecordsetsrequestpaginatetypedef) 
## ListVPCAssociationAuthorizationsPaginator

Type annotations and code completion for `#!python session.create_client("route53").get_paginator("list_vpc_association_authorizations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53/paginator/ListVPCAssociationAuthorizations.html#Route53.Paginator.ListVPCAssociationAuthorizations)

```python
# ListVPCAssociationAuthorizationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53.paginator import ListVPCAssociationAuthorizationsPaginator

session = get_session()
async with session.create_client("route53") as client:  # (1)
    paginator: ListVPCAssociationAuthorizationsPaginator = client.get_paginator("list_vpc_association_authorizations")  # (2)
    async for item in paginator.paginate(...):
        item: ListVPCAssociationAuthorizationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53Client](./client.md)
2. paginator: [ListVPCAssociationAuthorizationsPaginator](./paginators.md#listvpcassociationauthorizationspaginator)
3. item: [:material-code-braces: ListVPCAssociationAuthorizationsResponseTypeDef](./type_defs.md#listvpcassociationauthorizationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVPCAssociationAuthorizationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HostedZoneId: str,
    MaxResults: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVPCAssociationAuthorizationsResponseTypeDef](./type_defs.md#listvpcassociationauthorizationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVPCAssociationAuthorizationsRequestPaginateTypeDef = {  # (1)
    "HostedZoneId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVPCAssociationAuthorizationsRequestPaginateTypeDef](./type_defs.md#listvpcassociationauthorizationsrequestpaginatetypedef) 
