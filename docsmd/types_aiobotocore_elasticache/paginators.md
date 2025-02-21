# Paginators

> [Index](../README.md) > [ElastiCache](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElastiCache](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#elasticache)
    type annotations stubs module [types-aiobotocore-elasticache](https://pypi.org/project/types-aiobotocore-elasticache/).

## DescribeCacheClustersPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_cache_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeCacheClusters.html#ElastiCache.Paginator.DescribeCacheClusters)

```python
# DescribeCacheClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeCacheClustersPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeCacheClustersPaginator = client.get_paginator("describe_cache_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: CacheClusterMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeCacheClustersPaginator](./paginators.md#describecacheclusterspaginator)
3. item: [:material-code-braces: CacheClusterMessageTypeDef](./type_defs.md#cacheclustermessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCacheClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CacheClusterId: str = ...,
    ShowCacheNodeInfo: bool = ...,
    ShowCacheClustersNotInReplicationGroups: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[CacheClusterMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: CacheClusterMessageTypeDef](./type_defs.md#cacheclustermessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCacheClustersMessagePaginateTypeDef = {  # (1)
    "CacheClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCacheClustersMessagePaginateTypeDef](./type_defs.md#describecacheclustersmessagepaginatetypedef) 
## DescribeCacheEngineVersionsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_cache_engine_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeCacheEngineVersions.html#ElastiCache.Paginator.DescribeCacheEngineVersions)

```python
# DescribeCacheEngineVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeCacheEngineVersionsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeCacheEngineVersionsPaginator = client.get_paginator("describe_cache_engine_versions")  # (2)
    async for item in paginator.paginate(...):
        item: CacheEngineVersionMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeCacheEngineVersionsPaginator](./paginators.md#describecacheengineversionspaginator)
3. item: [:material-code-braces: CacheEngineVersionMessageTypeDef](./type_defs.md#cacheengineversionmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCacheEngineVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Engine: str = ...,
    EngineVersion: str = ...,
    CacheParameterGroupFamily: str = ...,
    DefaultOnly: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[CacheEngineVersionMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: CacheEngineVersionMessageTypeDef](./type_defs.md#cacheengineversionmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCacheEngineVersionsMessagePaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCacheEngineVersionsMessagePaginateTypeDef](./type_defs.md#describecacheengineversionsmessagepaginatetypedef) 
## DescribeCacheParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_cache_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeCacheParameterGroups.html#ElastiCache.Paginator.DescribeCacheParameterGroups)

```python
# DescribeCacheParameterGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeCacheParameterGroupsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeCacheParameterGroupsPaginator = client.get_paginator("describe_cache_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: CacheParameterGroupsMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeCacheParameterGroupsPaginator](./paginators.md#describecacheparametergroupspaginator)
3. item: [:material-code-braces: CacheParameterGroupsMessageTypeDef](./type_defs.md#cacheparametergroupsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCacheParameterGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CacheParameterGroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[CacheParameterGroupsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: CacheParameterGroupsMessageTypeDef](./type_defs.md#cacheparametergroupsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCacheParameterGroupsMessagePaginateTypeDef = {  # (1)
    "CacheParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCacheParameterGroupsMessagePaginateTypeDef](./type_defs.md#describecacheparametergroupsmessagepaginatetypedef) 
## DescribeCacheParametersPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_cache_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeCacheParameters.html#ElastiCache.Paginator.DescribeCacheParameters)

```python
# DescribeCacheParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeCacheParametersPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeCacheParametersPaginator = client.get_paginator("describe_cache_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: CacheParameterGroupDetailsTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeCacheParametersPaginator](./paginators.md#describecacheparameterspaginator)
3. item: [:material-code-braces: CacheParameterGroupDetailsTypeDef](./type_defs.md#cacheparametergroupdetailstypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCacheParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CacheParameterGroupName: str,
    Source: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[CacheParameterGroupDetailsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: CacheParameterGroupDetailsTypeDef](./type_defs.md#cacheparametergroupdetailstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCacheParametersMessagePaginateTypeDef = {  # (1)
    "CacheParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCacheParametersMessagePaginateTypeDef](./type_defs.md#describecacheparametersmessagepaginatetypedef) 
## DescribeCacheSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_cache_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeCacheSecurityGroups.html#ElastiCache.Paginator.DescribeCacheSecurityGroups)

```python
# DescribeCacheSecurityGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeCacheSecurityGroupsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeCacheSecurityGroupsPaginator = client.get_paginator("describe_cache_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: CacheSecurityGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeCacheSecurityGroupsPaginator](./paginators.md#describecachesecuritygroupspaginator)
3. item: [:material-code-braces: CacheSecurityGroupMessageTypeDef](./type_defs.md#cachesecuritygroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCacheSecurityGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CacheSecurityGroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[CacheSecurityGroupMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: CacheSecurityGroupMessageTypeDef](./type_defs.md#cachesecuritygroupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCacheSecurityGroupsMessagePaginateTypeDef = {  # (1)
    "CacheSecurityGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCacheSecurityGroupsMessagePaginateTypeDef](./type_defs.md#describecachesecuritygroupsmessagepaginatetypedef) 
## DescribeCacheSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_cache_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeCacheSubnetGroups.html#ElastiCache.Paginator.DescribeCacheSubnetGroups)

```python
# DescribeCacheSubnetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeCacheSubnetGroupsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeCacheSubnetGroupsPaginator = client.get_paginator("describe_cache_subnet_groups")  # (2)
    async for item in paginator.paginate(...):
        item: CacheSubnetGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeCacheSubnetGroupsPaginator](./paginators.md#describecachesubnetgroupspaginator)
3. item: [:material-code-braces: CacheSubnetGroupMessageTypeDef](./type_defs.md#cachesubnetgroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCacheSubnetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CacheSubnetGroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[CacheSubnetGroupMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: CacheSubnetGroupMessageTypeDef](./type_defs.md#cachesubnetgroupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCacheSubnetGroupsMessagePaginateTypeDef = {  # (1)
    "CacheSubnetGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCacheSubnetGroupsMessagePaginateTypeDef](./type_defs.md#describecachesubnetgroupsmessagepaginatetypedef) 
## DescribeEngineDefaultParametersPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_engine_default_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeEngineDefaultParameters.html#ElastiCache.Paginator.DescribeEngineDefaultParameters)

```python
# DescribeEngineDefaultParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeEngineDefaultParametersPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeEngineDefaultParametersPaginator = client.get_paginator("describe_engine_default_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEngineDefaultParametersResultTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeEngineDefaultParametersPaginator](./paginators.md#describeenginedefaultparameterspaginator)
3. item: [:material-code-braces: DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEngineDefaultParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CacheParameterGroupFamily: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeEngineDefaultParametersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeEngineDefaultParametersResultTypeDef](./type_defs.md#describeenginedefaultparametersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEngineDefaultParametersMessagePaginateTypeDef = {  # (1)
    "CacheParameterGroupFamily": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEngineDefaultParametersMessagePaginateTypeDef](./type_defs.md#describeenginedefaultparametersmessagepaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeEvents.html#ElastiCache.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: EventsMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SourceIdentifier: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Duration: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[EventsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventsMessageTypeDef](./type_defs.md#eventsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsMessagePaginateTypeDef = {  # (1)
    "SourceIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessagePaginateTypeDef](./type_defs.md#describeeventsmessagepaginatetypedef) 
## DescribeGlobalReplicationGroupsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_global_replication_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeGlobalReplicationGroups.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups)

```python
# DescribeGlobalReplicationGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeGlobalReplicationGroupsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeGlobalReplicationGroupsPaginator = client.get_paginator("describe_global_replication_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeGlobalReplicationGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeGlobalReplicationGroupsPaginator](./paginators.md#describeglobalreplicationgroupspaginator)
3. item: [:material-code-braces: DescribeGlobalReplicationGroupsResultTypeDef](./type_defs.md#describeglobalreplicationgroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeGlobalReplicationGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GlobalReplicationGroupId: str = ...,
    ShowMemberInfo: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeGlobalReplicationGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGlobalReplicationGroupsResultTypeDef](./type_defs.md#describeglobalreplicationgroupsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeGlobalReplicationGroupsMessagePaginateTypeDef = {  # (1)
    "GlobalReplicationGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGlobalReplicationGroupsMessagePaginateTypeDef](./type_defs.md#describeglobalreplicationgroupsmessagepaginatetypedef) 
## DescribeReplicationGroupsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_replication_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeReplicationGroups.html#ElastiCache.Paginator.DescribeReplicationGroups)

```python
# DescribeReplicationGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeReplicationGroupsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeReplicationGroupsPaginator = client.get_paginator("describe_replication_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ReplicationGroupMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeReplicationGroupsPaginator](./paginators.md#describereplicationgroupspaginator)
3. item: [:material-code-braces: ReplicationGroupMessageTypeDef](./type_defs.md#replicationgroupmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReplicationGroupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ReplicationGroupMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ReplicationGroupMessageTypeDef](./type_defs.md#replicationgroupmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationGroupsMessagePaginateTypeDef = {  # (1)
    "ReplicationGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationGroupsMessagePaginateTypeDef](./type_defs.md#describereplicationgroupsmessagepaginatetypedef) 
## DescribeReservedCacheNodesOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_reserved_cache_nodes_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeReservedCacheNodesOfferings.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings)

```python
# DescribeReservedCacheNodesOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeReservedCacheNodesOfferingsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeReservedCacheNodesOfferingsPaginator = client.get_paginator("describe_reserved_cache_nodes_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedCacheNodesOfferingMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeReservedCacheNodesOfferingsPaginator](./paginators.md#describereservedcachenodesofferingspaginator)
3. item: [:material-code-braces: ReservedCacheNodesOfferingMessageTypeDef](./type_defs.md#reservedcachenodesofferingmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedCacheNodesOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedCacheNodesOfferingId: str = ...,
    CacheNodeType: str = ...,
    Duration: str = ...,
    ProductDescription: str = ...,
    OfferingType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ReservedCacheNodesOfferingMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ReservedCacheNodesOfferingMessageTypeDef](./type_defs.md#reservedcachenodesofferingmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedCacheNodesOfferingsMessagePaginateTypeDef = {  # (1)
    "ReservedCacheNodesOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedCacheNodesOfferingsMessagePaginateTypeDef](./type_defs.md#describereservedcachenodesofferingsmessagepaginatetypedef) 
## DescribeReservedCacheNodesPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_reserved_cache_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeReservedCacheNodes.html#ElastiCache.Paginator.DescribeReservedCacheNodes)

```python
# DescribeReservedCacheNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeReservedCacheNodesPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeReservedCacheNodesPaginator = client.get_paginator("describe_reserved_cache_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ReservedCacheNodeMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeReservedCacheNodesPaginator](./paginators.md#describereservedcachenodespaginator)
3. item: [:material-code-braces: ReservedCacheNodeMessageTypeDef](./type_defs.md#reservedcachenodemessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedCacheNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedCacheNodeId: str = ...,
    ReservedCacheNodesOfferingId: str = ...,
    CacheNodeType: str = ...,
    Duration: str = ...,
    ProductDescription: str = ...,
    OfferingType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ReservedCacheNodeMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ReservedCacheNodeMessageTypeDef](./type_defs.md#reservedcachenodemessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedCacheNodesMessagePaginateTypeDef = {  # (1)
    "ReservedCacheNodeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedCacheNodesMessagePaginateTypeDef](./type_defs.md#describereservedcachenodesmessagepaginatetypedef) 
## DescribeServerlessCacheSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_serverless_cache_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeServerlessCacheSnapshots.html#ElastiCache.Paginator.DescribeServerlessCacheSnapshots)

```python
# DescribeServerlessCacheSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeServerlessCacheSnapshotsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeServerlessCacheSnapshotsPaginator = client.get_paginator("describe_serverless_cache_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeServerlessCacheSnapshotsResponseTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeServerlessCacheSnapshotsPaginator](./paginators.md#describeserverlesscachesnapshotspaginator)
3. item: [:material-code-braces: DescribeServerlessCacheSnapshotsResponseTypeDef](./type_defs.md#describeserverlesscachesnapshotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeServerlessCacheSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerlessCacheName: str = ...,
    ServerlessCacheSnapshotName: str = ...,
    SnapshotType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeServerlessCacheSnapshotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeServerlessCacheSnapshotsResponseTypeDef](./type_defs.md#describeserverlesscachesnapshotsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeServerlessCacheSnapshotsRequestPaginateTypeDef = {  # (1)
    "ServerlessCacheName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeServerlessCacheSnapshotsRequestPaginateTypeDef](./type_defs.md#describeserverlesscachesnapshotsrequestpaginatetypedef) 
## DescribeServerlessCachesPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_serverless_caches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeServerlessCaches.html#ElastiCache.Paginator.DescribeServerlessCaches)

```python
# DescribeServerlessCachesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeServerlessCachesPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeServerlessCachesPaginator = client.get_paginator("describe_serverless_caches")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeServerlessCachesResponseTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeServerlessCachesPaginator](./paginators.md#describeserverlesscachespaginator)
3. item: [:material-code-braces: DescribeServerlessCachesResponseTypeDef](./type_defs.md#describeserverlesscachesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeServerlessCachesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerlessCacheName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeServerlessCachesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeServerlessCachesResponseTypeDef](./type_defs.md#describeserverlesscachesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeServerlessCachesRequestPaginateTypeDef = {  # (1)
    "ServerlessCacheName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeServerlessCachesRequestPaginateTypeDef](./type_defs.md#describeserverlesscachesrequestpaginatetypedef) 
## DescribeServiceUpdatesPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_service_updates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeServiceUpdates.html#ElastiCache.Paginator.DescribeServiceUpdates)

```python
# DescribeServiceUpdatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeServiceUpdatesPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")  # (2)
    async for item in paginator.paginate(...):
        item: ServiceUpdatesMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeServiceUpdatesPaginator](./paginators.md#describeserviceupdatespaginator)
3. item: [:material-code-braces: ServiceUpdatesMessageTypeDef](./type_defs.md#serviceupdatesmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeServiceUpdatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceUpdateName: str = ...,
    ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ServiceUpdatesMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ServiceUpdatesMessageTypeDef](./type_defs.md#serviceupdatesmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeServiceUpdatesMessagePaginateTypeDef = {  # (1)
    "ServiceUpdateName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeServiceUpdatesMessagePaginateTypeDef](./type_defs.md#describeserviceupdatesmessagepaginatetypedef) 
## DescribeSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeSnapshots.html#ElastiCache.Paginator.DescribeSnapshots)

```python
# DescribeSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeSnapshotsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotsListMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeSnapshotsPaginator](./paginators.md#describesnapshotspaginator)
3. item: [:material-code-braces: DescribeSnapshotsListMessageTypeDef](./type_defs.md#describesnapshotslistmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReplicationGroupId: str = ...,
    CacheClusterId: str = ...,
    SnapshotName: str = ...,
    SnapshotSource: str = ...,
    ShowNodeGroupConfig: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSnapshotsListMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSnapshotsListMessageTypeDef](./type_defs.md#describesnapshotslistmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotsMessagePaginateTypeDef = {  # (1)
    "ReplicationGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsMessagePaginateTypeDef](./type_defs.md#describesnapshotsmessagepaginatetypedef) 
## DescribeUpdateActionsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_update_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeUpdateActions.html#ElastiCache.Paginator.DescribeUpdateActions)

```python
# DescribeUpdateActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeUpdateActionsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeUpdateActionsPaginator = client.get_paginator("describe_update_actions")  # (2)
    async for item in paginator.paginate(...):
        item: UpdateActionsMessageTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeUpdateActionsPaginator](./paginators.md#describeupdateactionspaginator)
3. item: [:material-code-braces: UpdateActionsMessageTypeDef](./type_defs.md#updateactionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUpdateActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceUpdateName: str = ...,
    ReplicationGroupIds: Sequence[str] = ...,
    CacheClusterIds: Sequence[str] = ...,
    Engine: str = ...,
    ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,  # (1)
    ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,  # (2)
    UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,  # (3)
    ShowNodeLevelUpdateStatus: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[UpdateActionsMessageTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: TimeRangeFilterTypeDef](./type_defs.md#timerangefiltertypedef) 
3. See [:material-code-brackets: UpdateActionStatusType](./literals.md#updateactionstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: UpdateActionsMessageTypeDef](./type_defs.md#updateactionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUpdateActionsMessagePaginateTypeDef = {  # (1)
    "ServiceUpdateName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUpdateActionsMessagePaginateTypeDef](./type_defs.md#describeupdateactionsmessagepaginatetypedef) 
## DescribeUserGroupsPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_user_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeUserGroups.html#ElastiCache.Paginator.DescribeUserGroups)

```python
# DescribeUserGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeUserGroupsPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeUserGroupsPaginator = client.get_paginator("describe_user_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUserGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeUserGroupsPaginator](./paginators.md#describeusergroupspaginator)
3. item: [:material-code-braces: DescribeUserGroupsResultTypeDef](./type_defs.md#describeusergroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUserGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserGroupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeUserGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeUserGroupsResultTypeDef](./type_defs.md#describeusergroupsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUserGroupsMessagePaginateTypeDef = {  # (1)
    "UserGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUserGroupsMessagePaginateTypeDef](./type_defs.md#describeusergroupsmessagepaginatetypedef) 
## DescribeUsersPaginator

Type annotations and code completion for `#!python session.create_client("elasticache").get_paginator("describe_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache/paginator/DescribeUsers.html#ElastiCache.Paginator.DescribeUsers)

```python
# DescribeUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticache.paginator import DescribeUsersPaginator

session = get_session()
async with session.create_client("elasticache") as client:  # (1)
    paginator: DescribeUsersPaginator = client.get_paginator("describe_users")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUsersResultTypeDef
        print(item)  # (3)
```

1. client: [ElastiCacheClient](./client.md)
2. paginator: [DescribeUsersPaginator](./paginators.md#describeuserspaginator)
3. item: [:material-code-braces: DescribeUsersResultTypeDef](./type_defs.md#describeusersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Engine: str = ...,
    UserId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeUsersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeUsersResultTypeDef](./type_defs.md#describeusersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUsersMessagePaginateTypeDef = {  # (1)
    "Engine": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUsersMessagePaginateTypeDef](./type_defs.md#describeusersmessagepaginatetypedef) 
