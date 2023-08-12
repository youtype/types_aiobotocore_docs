# Paginators

> [Index](../README.md) > [MemoryDB](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MemoryDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
    type annotations stubs module [types-aiobotocore-memorydb](https://pypi.org/project/types-aiobotocore-memorydb/).

## DescribeACLsPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_acls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeACLs)

```python
# DescribeACLsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeACLsPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeACLsPaginator = client.get_paginator("describe_acls")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeACLsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeACLsPaginator](./paginators.md#describeaclspaginator)
3. item: [:material-code-braces: DescribeACLsResponseTypeDef](./type_defs.md#describeaclsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeACLsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ACLName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeACLsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeACLsResponseTypeDef](./type_defs.md#describeaclsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeACLsRequestDescribeACLsPaginateTypeDef = {  # (1)
    "ACLName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeACLsRequestDescribeACLsPaginateTypeDef](./type_defs.md#describeaclsrequestdescribeaclspaginatetypedef) 
## DescribeClustersPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeClusters)

```python
# DescribeClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeClustersPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeClustersPaginator](./paginators.md#describeclusterspaginator)
3. item: [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterName: str = ...,
    ShowShardDetails: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClustersRequestDescribeClustersPaginateTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClustersRequestDescribeClustersPaginateTypeDef](./type_defs.md#describeclustersrequestdescribeclusterspaginatetypedef) 
## DescribeEngineVersionsPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_engine_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEngineVersions)

```python
# DescribeEngineVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeEngineVersionsPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeEngineVersionsPaginator = client.get_paginator("describe_engine_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEngineVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeEngineVersionsPaginator](./paginators.md#describeengineversionspaginator)
3. item: [:material-code-braces: DescribeEngineVersionsResponseTypeDef](./type_defs.md#describeengineversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEngineVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EngineVersion: str = ...,
    ParameterGroupFamily: str = ...,
    DefaultOnly: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeEngineVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeEngineVersionsResponseTypeDef](./type_defs.md#describeengineversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef = {  # (1)
    "EngineVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEngineVersionsRequestDescribeEngineVersionsPaginateTypeDef](./type_defs.md#describeengineversionsrequestdescribeengineversionspaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SourceName: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    Duration: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsRequestDescribeEventsPaginateTypeDef = {  # (1)
    "SourceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsRequestDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsrequestdescribeeventspaginatetypedef) 
## DescribeParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameterGroups)

```python
# DescribeParameterGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeParameterGroupsPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeParameterGroupsPaginator = client.get_paginator("describe_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeParameterGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeParameterGroupsPaginator](./paginators.md#describeparametergroupspaginator)
3. item: [:material-code-braces: DescribeParameterGroupsResponseTypeDef](./type_defs.md#describeparametergroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeParameterGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParameterGroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeParameterGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeParameterGroupsResponseTypeDef](./type_defs.md#describeparametergroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef](./type_defs.md#describeparametergroupsrequestdescribeparametergroupspaginatetypedef) 
## DescribeParametersPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeParameters)

```python
# DescribeParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeParametersPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeParametersPaginator = client.get_paginator("describe_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeParametersResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeParametersPaginator](./paginators.md#describeparameterspaginator)
3. item: [:material-code-braces: DescribeParametersResponseTypeDef](./type_defs.md#describeparametersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ParameterGroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeParametersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeParametersResponseTypeDef](./type_defs.md#describeparametersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeParametersRequestDescribeParametersPaginateTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeParametersRequestDescribeParametersPaginateTypeDef](./type_defs.md#describeparametersrequestdescribeparameterspaginatetypedef) 
## DescribeReservedNodesPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_reserved_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodes)

```python
# DescribeReservedNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeReservedNodesPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeReservedNodesPaginator = client.get_paginator("describe_reserved_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedNodesResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeReservedNodesPaginator](./paginators.md#describereservednodespaginator)
3. item: [:material-code-braces: DescribeReservedNodesResponseTypeDef](./type_defs.md#describereservednodesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservationId: str = ...,
    ReservedNodesOfferingId: str = ...,
    NodeType: str = ...,
    Duration: str = ...,
    OfferingType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReservedNodesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReservedNodesResponseTypeDef](./type_defs.md#describereservednodesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef = {  # (1)
    "ReservationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodesRequestDescribeReservedNodesPaginateTypeDef](./type_defs.md#describereservednodesrequestdescribereservednodespaginatetypedef) 
## DescribeReservedNodesOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_reserved_nodes_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodesOfferings)

```python
# DescribeReservedNodesOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeReservedNodesOfferingsPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeReservedNodesOfferingsPaginator = client.get_paginator("describe_reserved_nodes_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedNodesOfferingsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeReservedNodesOfferingsPaginator](./paginators.md#describereservednodesofferingspaginator)
3. item: [:material-code-braces: DescribeReservedNodesOfferingsResponseTypeDef](./type_defs.md#describereservednodesofferingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedNodesOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedNodesOfferingId: str = ...,
    NodeType: str = ...,
    Duration: str = ...,
    OfferingType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReservedNodesOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReservedNodesOfferingsResponseTypeDef](./type_defs.md#describereservednodesofferingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef = {  # (1)
    "ReservedNodesOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedNodesOfferingsRequestDescribeReservedNodesOfferingsPaginateTypeDef](./type_defs.md#describereservednodesofferingsrequestdescribereservednodesofferingspaginatetypedef) 
## DescribeServiceUpdatesPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_service_updates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeServiceUpdates)

```python
# DescribeServiceUpdatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeServiceUpdatesPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeServiceUpdatesResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeServiceUpdatesPaginator](./paginators.md#describeserviceupdatespaginator)
3. item: [:material-code-braces: DescribeServiceUpdatesResponseTypeDef](./type_defs.md#describeserviceupdatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeServiceUpdatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceUpdateName: str = ...,
    ClusterNames: Sequence[str] = ...,
    Status: Sequence[ServiceUpdateStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeServiceUpdatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceUpdateStatusType](./literals.md#serviceupdatestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeServiceUpdatesResponseTypeDef](./type_defs.md#describeserviceupdatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef = {  # (1)
    "ServiceUpdateName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeServiceUpdatesRequestDescribeServiceUpdatesPaginateTypeDef](./type_defs.md#describeserviceupdatesrequestdescribeserviceupdatespaginatetypedef) 
## DescribeSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSnapshots)

```python
# DescribeSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeSnapshotsPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeSnapshotsPaginator](./paginators.md#describesnapshotspaginator)
3. item: [:material-code-braces: DescribeSnapshotsResponseTypeDef](./type_defs.md#describesnapshotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterName: str = ...,
    SnapshotName: str = ...,
    Source: str = ...,
    ShowDetail: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSnapshotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSnapshotsResponseTypeDef](./type_defs.md#describesnapshotsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef](./type_defs.md#describesnapshotsrequestdescribesnapshotspaginatetypedef) 
## DescribeSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSubnetGroups)

```python
# DescribeSubnetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeSubnetGroupsPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeSubnetGroupsPaginator = client.get_paginator("describe_subnet_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSubnetGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeSubnetGroupsPaginator](./paginators.md#describesubnetgroupspaginator)
3. item: [:material-code-braces: DescribeSubnetGroupsResponseTypeDef](./type_defs.md#describesubnetgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSubnetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SubnetGroupName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSubnetGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSubnetGroupsResponseTypeDef](./type_defs.md#describesubnetgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = {  # (1)
    "SubnetGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef](./type_defs.md#describesubnetgroupsrequestdescribesubnetgroupspaginatetypedef) 
## DescribeUsersPaginator

Type annotations and code completion for `#!python session.create_client("memorydb").get_paginator("describe_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeUsers)

```python
# DescribeUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_memorydb.paginator import DescribeUsersPaginator

session = get_session()
async with session.create_client("memorydb") as client:  # (1)
    paginator: DescribeUsersPaginator = client.get_paginator("describe_users")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [MemoryDBClient](./client.md)
2. paginator: [DescribeUsersPaginator](./paginators.md#describeuserspaginator)
3. item: [:material-code-braces: DescribeUsersResponseTypeDef](./type_defs.md#describeusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserName: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeUsersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeUsersResponseTypeDef](./type_defs.md#describeusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUsersRequestDescribeUsersPaginateTypeDef = {  # (1)
    "UserName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUsersRequestDescribeUsersPaginateTypeDef](./type_defs.md#describeusersrequestdescribeuserspaginatetypedef) 
